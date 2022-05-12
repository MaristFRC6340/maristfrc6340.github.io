## Version Control for Robot Code

Version control, or the ability to record changes to a file or set of files over time in a group setting, is used commonly in FRC to be able to have a single
code base that programmers can retrieve from the cloud, make changes locally (i.e. in [Visual Studio Code](https://code.visualstudio.com/), then upload their changes
back to the cloud.

In this blog post, you will learn out to:
* Create a repository in the Marist FRC 6340
* Connect to it in VS Code on the Marist Robotics Macs
* Upload changes back to the repository

---

The first thing to understand are the essential concepts of version control and [Git](https://git-scm.com/), a version control tool built into the VS Code user interface.

Instead of me explaining it, I recommend clicking on this YouTube video below:

[![what is git and github yt](https://img.youtube.com/vi/uUuTYDg9XoI/mqdefault.jpg)](https://www.youtube.com/watch?v=uUuTYDg9XoI)

Here is a table with the buttons/commands that you will use with Git (at least in this environment because there are TONS of more Git features):

| Command | Description |
| --- | ----------- |
| Add Changes | When you make changes to the lines of code in your project, add these changes so they are "tracked" in Git |
| Commit | In order to group line-by-line changes together, you make a commit once you have added the changes you want. You will specify a name for the commit |
| Push | Once you make a commit, push your changes to the repository in the cloud
| Pull/Fetch | If you have made no changes from the *last pushed commit* in the repository, fetch the changes locally that someone else may have uploaded to Github
| Clone | Download the repository, aka project, from the cloud, aka github.com, with version control already enabled and ready to use

---

> **Create repository**
1. Follow [this](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository) guide on creating a repository on your github account
2. However, when you get to the page where you specify the details of the repository (step 2 and on), make sure to press the `Owner` dropdown and select `MaristFRC6340`

> **Clone repository in VS Code on FRC Programming Computer**
1. Follow [this](https://code.visualstudio.com/docs/editor/github#_cloning-a-repository) guide
2. If the repository you just made does not show up in dropdown, go back to your Github repository, press the green `code` button, copy the .git link, and paste it into the VS Code dropdown

> **Add changes**
1. Once you are finished coding, go to the Source Control panel (see image below)
2. Press the plus for every file you want to add changes for or press the plus in the container to add them all with one button

![image](https://user-images.githubusercontent.com/44009231/167955938-cd01e535-ce51-4774-b887-aed6da1d76e4.png)


> **Commit changes**
1. In the text box near the top of the Source Control Panel, type the commit message
2. Read [this article](https://code.visualstudio.com/docs/editor/versioncontrol#_commit) for more information

> **Push changes
1. Click on the three dots, which is the menu for `Views and More Actions`
2. Press the `Push` button

![image](https://user-images.githubusercontent.com/44009231/167966154-164c48f9-f291-4f25-bd9c-920a45392d91.png)

---

### Things to consider

These instructions assume that you are creating a whole new, blank repository then creating the WPILib code locally in VS Code.

*However,* you might be instead trying to get someone else's MaristFRC6340 repository into VS Code. In this case, you can skip the first step, `Create Repository`,
and instead clone the repository from Github.

To do this, you simply press on the green `Code` button on the Github page for the repository you want to clone. Then, copy the .git link and back in VS Code,
in the Source Control Panel, click `Clone Repository`, and paste that copied link in the following text box. All steps after that still work!

> NOTE: for those who want to clone a repository outside of the Marist 6340 organization, ask [Alessio Toniolo](https://github.com/AlessioToniolo)

---

<h4 align="center"> Created by Alessio Toniolo </h4>
