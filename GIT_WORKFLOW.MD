# Basic commands for git flow

Partially taken from:
* [Cloning-the-repo-and-working-with-Git](https://github.com/GarageGames/Torque2D/wiki/Cloning-the-repo-and-working-with-Git)
* [Syncing fork with original repo](https://digitaldrummerj.me/git-syncing-fork-with-original-repo/)

## Creating a Fork
Check out this [link](https://help.github.com/en/github/getting-started-with-github/fork-a-repo) if you don't know how to fork a repository 

## One-time setup 

#### Globally configure your username (if not done so already)

```$ git config --global user.name "Your Name here"```


#### Golbally configure your email of github account (if not done so already)

```$ git config --global user.email "your_email@domainname.com"```


#### Cloning via ssh (pattern: <i>git@github.com:your_username/forked_repo_name</i>)

```$ git clone <repository_name>```


#### Very important, in order to pull code from original repo:

(where <repo_name> is original repo name)
```$ git remote add upstream git@github.com:agno-ai/<repo_name>```


#### Then fetching changes from original repo

```$ git fetch upstream```


#### Finally merging changes from original repo with forked repo

```$ git merge upstream/master```


## Normal Git Flow Starts Here

Work on your code...

#### Pull local changes

```$ git pull```

#### Pull changes from original repo

```$ git fetch upstream```


#### Merge changes from original repo into local forked repo

```$ git merge upstream/master```


#### add your changes

```$ git add .```


#### create a commit with a message

```$ git commit -m "Add a mandatory message"```


#### push your code

```$ git push ```



