## Our version of [Plants vs Zombies](https://www.ea.com/studios/popcap/plants-vs-zombies) in Python 3

For Mannie: to create your own copy of this repository folder, click the 'Fork' button at the top right corner (next to the 'Unwatch' and 'Star' buttons). The new copy will be located at [this address](https://github.com/manniepmkam/PvZ).

to create a local copy of this repository folder, navigate to the address where you want to store this local copy, and then run the following in the command line: `git clone git@github.com:manniepmkam/PvZ.git`

Next, if you run `git branch`, you should see that you are on your `master` branch. Please do **not** commit any changes to the `master` branch directly. Instead, switch to another branch for development purposes by running:

```
git branch develop-pm
git checkout develop-pm
```
If you run `git branch` again, you should see that you are now on the development branch. Please do also create a new remote for the original repository folder by running: `git remote add upstream https://github.com/liweiyap/PvZ.git`.

Now, every time you open your local copy to work, you want to make sure that your local copy is synced with mine. To do so, run:
```
git pull upstream master
git push origin master
```
Here, `upstream` refers to my original repository, whereas `origin` refers to your copy. You are pulling from my `master` branch and pushing to your own `master` branch.

<p align="center">
  <img src="https://images.osteele.com/2008/git-transport.png">
</p>

Assuming that we have a file called `hello-world.py`, and we have separately made so many changes that there are conflicts during syncing, run [`git mergetool`](https://stackoverflow.com/questions/161813/how-to-resolve-merge-conflicts-in-git) to see the differences between our versions of this file. (Another option would be: [`git diff --word-diff`](https://git-scm.com/book/en/v2/GitHub-Contributing-to-a-Project).) If you decide to use your own changes, run `git checkout --ours hello-world.py`. Otherwise, run `git checkout --theirs hello-world.py`. Then, run the following:
```
git add hello-world.py
git commit -m "[Replace this custom message with your own.]"
```
Now, if you run `git pull upstream master` again, the syncing error will have disappeared. To update your local copy of the repository, run `git fetch origin master` and then `git status` to decide which commits to merge.

To merge the changes in your `master` branch with your development branch, first add and commit the current changes in your development branch, and then push them to your fork of the repository by running: `git push origin develop-pm`. Now, go back to your fork on the GitHub website and create a new pull request to your `master` branch.

Finally, to inform me about any changes that you have made, go to my original repository on the GitHub website and create a new pull request to my `master` branch, so that I can merge the changes.

Let's test this soon.
