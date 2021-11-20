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
You can check status of your repo by using:
```
git status
```

If you want to commit to local repo, using this command:
```
git commit -m "your comment for commit here"
```

If you add new file after you init project, git will not add that file to index. You need to add file first.
```
git add {filename}

//for example
git add README.txt //add README.txt to index
git add *.txt //add all files that have ".txt" to index
git add * //add all files(not recommends)
```

Use `git log` to check commit logs.
Use `git ls-files` to check files in the index

## Link to github
First, you need to create github account and create new repo, then you copy link of your repo. Then in local repo use this commands.
```
git branch -M main
git remote add origin {repo link}
```

Then you use this commands to upload repo to github.
```
git push -u origin main //first time only
git push //use this commands next times
```

**IMPORTANT: You need to `commit` latest version of your project to local repo before `push` to github.**

Then go to your github repo and check your repo are up to date.

(END)

-----
vscode custom settings(add in .vscode/settings.json)
saved for using later
```
{
  "files.autoSave": "afterDelay",
  "editor.fontFamily": "Fira Code",
  "editor.fontLigatures": true,
  "editor.cursorBlinking": "expand",
  "editor.fontWeight": "400"
}
```
