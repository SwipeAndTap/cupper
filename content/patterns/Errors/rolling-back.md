+++
title="Rolling Back"
weight = 1
+++

## Reverting ##

If ever you need to go back to a previous commit, the recommended way is using the `revert` keyword with the commit id 
that you would like to revert to:

{{<cmd>}}
git revert [commit-id]
{{</cmd>}}

This will firstly revert your current branch to that particular commit but will not lose the history between. It will 
create a new commit for the reversion which is a safe way to undo code.

## Resetting ##

Another useful but sometimes dangerous command is `reset`.  
This can be used to undo files in the staging area if they were accidentally added. This can be done with:
{{<cmd>}}
git reset [file-name]
{{</cmd>}}
To unstage a particular file. 

OR

{{<cmd>}}
git reset
{{</cmd>}}
To reset all files from the staging area.

This will leave the actually code as it is but simply take the staging back to where the previous commit was.

The other thing to consider is the `—hard` flag which performs the same job as above but actually resets the code in the 
selected file(s) to what was in the last commit, thus losing any changes you have made since.  
Using hard resets should only be performed in an absolute emergency or only if you know what you are doing.