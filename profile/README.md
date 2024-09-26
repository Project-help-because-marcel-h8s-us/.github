# A helping hand with the first project

## Hi there 👋. Lets Get started

There are two options for setting up your repo here. One is the easier choice the other is a little more advanced. Both require a small thing to remember

## Option 1 - Create a copy

1. clone the empty repo from the github page with `git clone <repo url>`
2. copy your project into the repo
4. ```
   git add .
   git commit -m "Initial commit"
   git push
   ```

Just remember to move your changes across to the original folder to push them to the school server

## Option 2 - add a git remote

Option 2 is a little more complex but is good practice. The idea is to add a second git remote along side your gitlab server.
The danger here is that the changes may not be in sync across the different remote locations and merge changes could become a difficult challenge.

But if you're up to the challenge you can give it a try

**Setup**:
In your project git repo on your machine run the command:
  ```
git remote add <name> <url>
```
where `name` is a name of your choosing and `url` is the link to the github repo here.


This will set up a second remote location. So when you push, pull and fetch you can do it to two places.

The command:
```
git push --all
```
will do this. But if you want to push to just one of the repos you can use:
```
git push <name> 
```
where `name` is the name you chose in the earlier git add command.

the command:
```
git push origin
```
will most likely push your code to the gitlab server but you can use:
```
git remote -v 
```
will list the urls names of the remote locations you have setup if you want to make sure.
