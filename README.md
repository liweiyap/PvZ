## Our version of [Plants vs Zombies](https://www.ea.com/studios/popcap/plants-vs-zombies) in Python 3

For Mannie: to create your own copy of this repository folder, click the 'Fork' button at the top right corner (next to the 'Unwatch' and 'Star' buttons). The new copy will be located at [this address](https://github.com/manniepmkam/PvZ).

to create a local copy of this repository folder, navigate to the address where you want to store this local copy, and then run the following in the command line: `git clone git@github.com:manniepmkam/PvZ.git`

Next, if you run `git branch`, you should see that you are on the master branch. Please do **not** commit any changes to this branch directly. Instead, switch to another branch for development purposes by running:

```
git branch develop-pm
git checkout develop-pm
```
If you run `git branch` again, you should see that you are now on the development branch. Please do also create a new remote for the original repository folder by running: `git remote add upstream https://github.com/liweiyap/PvZ.git`.
