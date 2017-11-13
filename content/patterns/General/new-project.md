+++
title = "Create New Project"
weight = 1
+++

When a new project is ready to be implemented, a new empty private repository will be created on the [Swipe & Tap GitHub account](https://github.com/SwipeAndTap)

A designated user will then initialise the directory structure based on the selected framework and push to the remote origin using the following steps:

1. Create a local directory to store the project:
{{<cmd>}}
    mkdir [project]
{{</cmd>}}

2. Initalise local git repository using the following command:
{{<cmd>}}
    git init
{{</cmd>}}

3. Initialise project structure and perform an initial commit

4. Reference the github repository as your remote origin
{{<cmd>}}
    git remote add origin https://github.com/SwipeAndTap/project.git
{{</cmd>}}

5. Push all of the inital code to the remote Github repository
{{<cmd>}}
    git push -u origin master
{{</cmd>}}

{{<note>}}
    [project] refers to the name of the folder you would like to create the project within
{{</note>}}

Other users can now {{% pattern "Clone Existing Project" %}}.