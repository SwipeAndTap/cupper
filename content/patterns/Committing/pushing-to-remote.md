+++
title="Pushing to Remote Branch"
weight = 2
+++

Eventually, the changes made locally will have to be pushed to the online repository both for backup purposes and also 
for members to be able to actively see progress across the team for those working on the same area.

At a minimum, all local commits should be pushed at least **twice a day**, once before lunch and once before leaving the 
office. There is no limit on the number of pushes to the remote branch per day, but these two times are recommended for 
many reasons:
  
- If you leave for lunch and another member is working closely on a related piece of a feature, they will have to wait 
for you to return to be able to ask any questions.
- If there is an emergency such as a fire during the day, the risk of losing work is reduced to half a day at most.
- If there is a problem outside of work hours such as computer breaks, is stolen or any other disaster occurs, you will 
have no local work that needs to be recovered and can be picked up where left off

To push commits to the remote branch, you can use:

{{<cmd>}}
git push origin [branch-name]
{{</cmd>}}

{{<note>}}
If the branch name that you push does not already exist in the remote repository, it will automatically be created.
Otherwise, the named branch will be updated with the changes.
{{</note>}}

Once the work on the feature branch has been completed, the next step is to consider {{% pattern "Pull Requests" %}}.