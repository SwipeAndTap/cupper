+++
title="Committing Locally"
weight = 1
+++


As the first step, committing work locally should be a consistent part of your workflow which will help in many ways 
such as keeping related code together and creating a history that reduces risk in the event of reverting code.

## Commit Messages ##
A good history is only as good as its commit messages. Being descriptive will help to make the timeline more readable 
and understandable for team members.

The simplest way to stage and commit changes is as follows:

{{<cmd>}}
git add .
{{</cmd>}}
{{<cmd>}}
git commit -m “message”
{{</cmd>}}


This will firstly stage all files within the commit, followed by committing those files with the inserted message.

To stage files individually, you can replace the “.” character with the relative path the the file you would like to 
stage.
Doing it by file it effective when you need to split a lot of changes into more digestible commits.

Messages should be in the present tense and begin with a verb. An accepted practice is to structure your message to 
extend the following statement:

*"If applied, this commit will…"*

Other guidelines to consider are:

- Summarise the changes by limiting the message to 50 characters
- Concentrate on explaining WHAT has changed as opposed to WHY
- Capitalise the first letter of the summary 

If you’re having a hard time summarising, you might be committing too many changes at once. See [Frequency](#frequency) 
section for help on this.

## Frequency ##

How often you commit code can have a great effect on its history and how easy it is to follow. This will help both you 
and your team over time to understand the features that you are developing.
Though it may be overkill to commit after each line of code, it should ideally be **multiple times a day**.

As a general guideline, code should be committed **as each subset of a feature is completed**.  
This way, commit messages can be kept short and concise and will keep highly related code within the same commit.

To make sure the remote repository contains the newest code commits, you can start {{% pattern "Pushing to Remote Branch" %}}.