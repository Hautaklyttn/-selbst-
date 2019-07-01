---
layout: default
---

&nbsp;

1. TOC
{:toc}

&nbsp;

***

==>[ Git Basics](./git_basics.html)

***

&nbsp;

<font size="-1"><span style="color:green">- Step 1 -</span></font>
# _Set the project base with CM_Template_
&nbsp;

### Create an empty repository on GitHub in 'VED_CarMaker-HiL'

1. Click &nbsp;&nbsp;![Fork](/assets/images/new.png)
2. Enter <span style="color:LimeGreen ">Repository Name</span> - Usually the name of the customer project
3. Add <span style="color:LimeGreen">Description</span> (e.g. _The repository for the ... HIL simulation project._)
4. Select <span style="color:LimeGreen">Public</span> repository
5. Select <span style="color:LimeGreen">Initialize this repository with a README</span> (adds an inital README to the project)

> Result is an empty repository (except README.md) . This will be our <span style="color:LimeGreen">upstream</span> repository.

&nbsp;

### 'Fork' the repository to your GitHub account

1. Click &nbsp;&nbsp;![Fork](/assets/images/fork.png)
2. Select your account.

> Result is a forked repository on your GitHub account. This will be our <span style="color:LimeGreen">origin</span> repository.

&nbsp;


### 'Clone' the forked repository

1. Click &nbsp;&nbsp;![Fork](/assets/images/clone.png)
2. Select &nbsp;&nbsp;![Fork](/assets/images/https.png) &nbsp;&nbsp; and click on the 'Copy' icon &nbsp;&nbsp;![Fork](/assets/images/copy.png)
3. Open 'SmartGit' and open menu entry <span style="color:LimeGreen">Repository -> Clone</span>
4. Copy URL to <span style="color:LimeGreen">Repository URL</span> (if not already present)
5. Click 'Next' (2x), select the location for your local Sandbox and click <span style="color:LimeGreen">Finish</span>

> Result is a local repository (or Sandbox) on your machine.

&nbsp;


### Add 'Remotes'

1. Open menu entry <span style="color:LimeGreen">Remote -> Add..</span>
2. - for <span style="color:LimeGreen">upstream</span>
      - Go to our <span style="color:LimeGreen">upstream</span> repository on GitHub and do the steps 1. and 2. from step [_'Clone' the forked repository_]
      - Copy the link to <span style="color:LimeGreen">URL or Path</span>
      - Enter <span style="color:LimeGreen">upstream</span> as <span style="color:LimeGreen">Name</span>
   - for <span style="color:LimeGreen">cm_template</span>
      - Go to 'VED-CarMaker-HIL/CM_Template' on GitHub and do the steps 1. and 2. from step [_'Clone' the forked repository_]
      - Copy the link to <span style="color:LimeGreen">URL or Path</span>
      - Enter <span style="color:LimeGreen">cm_template</span> as <span style="color:LimeGreen">Name</span>

> Result are two additional remote locations your local copy can <span style="color:LimeGreen">Push to</span> or
<span style="color:LimeGreen">Pull from</span> later on.

&nbsp;


### Pull 'CM_Template' as your base project

Our future project is supposed to be based on a common project structure with the most recent additions and fixes.
This can be found in the repository <span style="color:LimeGreen">CM_Template</span>.

1. Because there are two 'README.md' files when we <span style="color:LimeGreen">Pull</span> from the base project, there is a conflict ahead.
Open the Git shell in Smart Git (<span style="color:LimeGreen">Tools -> Git Shell</span>) and enter
```git
git pull --progress -v --no-rebase --allow-unrelated-histories "cm_template" master
```
Now all files should be copied to your local drive.
2. <span style="color:LimeGreen">Remove</span> the empty 'README.md' file and <span style="color:LimeGreen">Stage</span> (=Add) the 'README.md' from 'CM_Template'
3. <span style="color:LimeGreen">Commit</span> and <span style="color:LimeGreen">Push</span> everything to your 'fork' (=<span style="color:LimeGreen">origin</span>)
4. In your 'fork' on GitHub click &nbsp;&nbsp;![Fork](/assets/images/pullReq.png) &nbsp;&nbsp; to create a merge request
of the 'CM_Template' contents to the <span style="color:LimeGreen">upstream</span>

> Result is a basis for the project setup with the most recent additions on all locations.

&nbsp;


### Ready for Project setup

Now all preparation steps are done and we can start with the actual project setup.
Go to your local repository and set up the project on top of the template (see next Chapter<span style="color:yellow"> 'Project Setup')</span>.
&nbsp;

In the end, after making sure the project is compiling, <span style="color:LimeGreen">Push</span> everything to your 'fork' and
make a <span style="color:LimeGreen">Pull Request</span> to the <span style="color:LimeGreen">upstream</span>.
&nbsp;

> When the project is done and rolled out, make sure to <span style="color:LimeGreen">Pull</span> from <span style="color:LimeGreen">cm_template</span>
 from time to time to be up-to-date with basic project updates/additions.

&nbsp;

&nbsp;

<font size="-1"><span style="color:green">- Step 2 -</span></font>
# _Project Setup_



&nbsp;

***

&nbsp;

[Link to styles](./another-page.html)


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<font size="+3"><span style="color:red"> !!! PAGE UNDER CONSTRUCTION !!!</span></font>
&nbsp;
