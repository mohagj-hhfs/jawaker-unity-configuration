# Git

[Git](https://git-scm.com/) is a version control system. We use it (along with github) to do all of our work

## Resources
Here are two resources that will help you better understand git:
- [Git Handbook](https://guides.github.com/introduction/git-handbook/)
- [Git Interactive Tutorial](https://learngitbranching.js.org/)

## Installation
If you already installed iTerm, simply entering this command and hitting enter on the terminal will prompt you to install git
```bash
git
```

After you have git, we need to go now to Github

# Github

Github is where we store our code, and everyone pushes and pull code from it. If you don't already have an account, please create one now - beware that it should be connected to your PERSONAL email and not the one provided by the company. After you created your account, do the following steps:
- [Generate an ssh key](https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
- [Add the key to your Github account](https://help.github.com/en/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account)

After that we will connect our local git  client with our github account, open a terminal and do the following:
```bash
git config --global user.name 'Your github username'
git config --global user.email 'Your github email'
```
