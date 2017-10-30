# Git Utils

## prepare-commit-msg

#### Add a precommit message to the git commit.

Create a file **_prepare-commit-msg_** in the .git/hooks folder of the repo. And after you create it you need to make that file executable. To do so, run the command
 
 > chmod +x .git/hooks/prepare-commit-msg 
  
For example, if your branch name is *ABC-123/feature* (where ABC-123 is the jira tag), when you commit something using git commit -m "your message", this little script appends the jira tag to it.

Now your commit looks like this. 

> ABC-123: Your commit message....
