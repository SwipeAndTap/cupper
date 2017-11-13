+++
title = "Feature Branches"
weight = 2
+++

## Creating a branch ##

As stated in the {{% pattern "Constant Branches" %}} section, the Development branch will be the root branch of the 
project lifecycle yet it should not be worked on directly.

For each major feature within the system, a new independent branch should be created (see [Naming Conventions](#naming-conventions)) 
from the dev branch. This can be done by using the following command (making 
sure that the current branch is dev):

{{<cmd>}}
git checkout -b [branch-name]
{{</cmd>}}

{{<note>}}
    [branch-name] refers to the name of the branch you are creating
{{</note>}}

This command will both create a new branch and also checkout that branch so that it can be immediately worked on.

Following on from here, development can begin on the feature using the continued flow mentioned in sections 
{{% pattern "Committing" %}} and {{% pattern "Merging" %}}.

## Naming conventions ##

The naming conventions illustrated here are merely guidelines but should help to structure feature branches in a way that can be understood by all members of a team working on a project.

Feature branches should use the following conventions where appropriate:

- Words should only contain lowercase letters
- A hyphen should be used between words if more than 1
- Branch name should describe the feature in plain English in as minimum words as possible
- If branch relates to an API, it should be prefixed with `api/`
- If branch relates to previous feature, the name should match and be appended with an appropriate word such as `fix` or `updates`

## Examples ##

**Feature**
A web dashboard overview of system users.  
**Branch** 
`users-dashboard`

**Feature**
Improved designs for a form that is used for adding inventory which is an existing feature  
**Branch**
`inventory-updates`

**Feature**
APIs for getting and adding new patient details for a hospital  
**Branch** 
`api/patients`

Once the branch is in place and coding a feature has begun, you can start {{% pattern "Committing Locally" %}} to continue the workflow.