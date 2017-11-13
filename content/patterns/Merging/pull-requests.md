+++
title="Pull Requests"
weight = 1
+++

## Pull Request ##

Creating a pull request for a feature branch will help to make sure that everything merged to the development branch is 
of a good coding standard and also reaches the intended goal, as well as helping to maintain an accurate and descriptive 
commit history that takes into account the branch that was merged in.

Pull requests are also a great way to start a conversation relating to a feature, allowing users to talk through any 
questions and ideas before continuing with development.
Users can also review the code in a number of useful ways.

You can create pull requests on a repository on the GitHub site:

1. Click on the *Branches* button under the *Code* tab
2. Find the branch you would like to submit a pull request from and click *New Pull Request*
3. If needed, you can select a branch to merge into from the *base* dropdown if this does not apply to the default branch
4. Fill out the comment if needed followed by clicking *Create Pull Request* or you may assign a reviewer first by 
referring to [Assigning Users](#assigning-users) section

{{<note>}}
It is highly recommended to enter a comment before creating a pull request.
The comment should consist of a plain English (non-technical) explanation of what the branch consists of. This is so 
that any other members involved - particularly the reviewer - will have an understanding of what to expect from the code 
before they dive in.
{{</note>}}

To make things easier for the reviewer or other assignees, if standards were followed throughout the git process, the 
branch name, request comment and commit messages should provide an easy way for them to navigate around and understand 
the purpose of everything here.

## Assigning Users ##

When creating or viewing a pull request, it is possible to add any number of users as a reviewer in order to notify them 
that the code is ready to be reviewed.

Simply click on the cog to the right of the *Reviewers* section to the right of the request details and enter the name 
of the user to assign.

They will then receive an email prompting them that they have been assigned to review the pull request.

## Review ##

The real benefit of a pull request is for other specified users to be able to perform detailed reviews relating to a 
submitted branch. This could simply be skimming through the code, or more advanced tasks such as leaving comments and 
highlighting lines of code to be fixed or improved.

A reviewer can either leave comments, approve the code or request changes to be addressed before the branch is deemed 
suitable to merge.

If there are any conflicts in the code, then take a look at {{% pattern "Merge Conflicts" %}}.

Otherwise, you can {{% pattern "Merge and Cleanup" %}} .