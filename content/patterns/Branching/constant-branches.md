+++
title = "Constant Branches"
weight = 1
+++

Each project will always begin with the following 2 branches that will remain active throughout the entire project (and 
beyond).

## Master ##

The master branch that is automatically introduced with new GitHub projects will be the starting point for all 
development. 

This is intended to be the most stable branch of all, which will be used in the live production environment of the 
client.
This means that all code that is merged to it will have been thoroughly tested and approved before getting to this 
constant stage.

{{<warning>}}
The only time you should commit to the master branch is when merging the dev branch into it.
{{</warning>}}

## Dev/Development ##

From the master branch, a secondary branch will be created to be the base for all development throughout the project.

Though this branch should remain stable, having it separate from the master branch will allow testing features and 
fixing bugs to be isolated from the production environment.  
Therefore, when the dev branch is stable, it can be safely merged into the master branch assuming it has been tested and 
reviewed as necessary.

Team members should not work directly on this branch but should create separate feature branches that are eventually 
added as pull requests and merged into this branch when completed.  

This process is outlined in the {{% pattern "Feature Branches" %}} section.