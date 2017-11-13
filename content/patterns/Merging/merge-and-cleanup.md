+++
title="Merge and Cleanup"
weight = 3
+++

Once any changes have been mad, review is approved and the branch has no merge conflicts, a user can successfully merge 
the pull request.

Once the branch is merged, a purple icon will show that status on github. At this point, you should delete the branch 
unless further work will continue on the branch.
If you have finished with the branch and choose to delete it, you can update your local environment as follows:

1. Checkout the branch that the current feature branch was merged into
2. Pull the committed merge:
{{<cmd>}}
git pull origin [branch]
{{</cmd>}}

3. Safely delete the feature branch that was merged:
{{<cmd>}}
git branch -d [feature-branch]
{{</cmd>}}

{{<note>}}
Note the lowercase -d in the above command. This is a safe delete option that will only delete the feature branch if it 
has been merged.
If this does not work and you are completely sure that you no longer need the local branch, you can override this using 
a capital -D instead
{{</note>}}

If you have any issues at this stage, it might be useful to look at different ways of {{% pattern "Rolling Back" %}}.