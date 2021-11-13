# git101
git setup for any project
(This is my lecture, not about workshop)
## Add git to your project
First you need to install **git** in your computer.

Then you open cmd/shell at your project and run command
```
git init
```

Next you need to add a username and email for Your Identity. It important to add identity because git use this info to save uour commits.
```
git config user.name "username"
git config user.email "email@mail.com
```

on above commands only config at local project only. If you want to make your account to global, you need to declare `--global` variable, for exammple:
```
git config --global user.name "username"
```

then you can use `git config --list` to check your settings.
## First commit
you can check status of your repo by using:
```
git status
```

First you donnt see any
```
git commit -m "your comment for commit here"
```
<-m> is 