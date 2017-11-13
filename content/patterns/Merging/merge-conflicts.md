+++
title="Merge Conflicts"
weight = 2
+++

If there are any merge conflicts at this point, they must be solved before merging the pull request to the requested 
branch. 

For simple merge conflicts, you have the ability to use the web editor to fix them by going through the list of files 
with merge conflicts and looking for the following the following lines:
```
<<<<<<< HEAD
=======
>>>>>>> branch-name
```  
This splits the current branch and merging branch to show the
differences between the files. Simply remove the conflict characters and leave the code that is correct.

For more complex conflicts you must use the command line to solve them. This involves viewing the files in your editor 
of choice and manually going through and committing the fixes back onto the same branch. When this is completed, it can 
be pushed and the conflicts should no longer show in the pull request.

When the conflicts have been solved, it's time to {{% pattern "Merge and Cleanup" %}}.