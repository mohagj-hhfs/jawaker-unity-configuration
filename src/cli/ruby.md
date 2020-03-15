# Ruby

Ruby is general purpose scripting language. Although we're going to do any development using ruby, we still need it to power some of the tools we'll be using along Unity

# Rbenv

Rbenv is a tool that makes managing ruby versions between projects easy, and saves lots of the overhead with dealing with all its ecosystem. 
To install rbenv:
```bash
brew install rbenv
```
And then, if you don't have a .bash_profile then create one
```bash
cd
touch .bash_profile
```
and then open the .bash_profile and put this in it:
```
eval "$(rbenv init -)"
```

and then in the terminal:
```bash
source ~/.bash_profile
```
