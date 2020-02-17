# Reviewing in markdown and git
This document outlines where to start and what to do to get going when reviewing content. It is the next step after the authoring with markdown and git guide. It will not provide all details, rather, it will provide details around the process and tools usage for authoring, commands and basic procedures to achieve certain tasks, as well as outlining some best practices.

## Prerequisites

- Follow this guide after you complete the **Author quick start guide**. The **Author quick start guide** is available [from the project's Teams site](https://teams.microsoft.com/l/file/DE9F6B1E-37E1-487D-A4E6-D6BB1E3A4C69?tenantId=4f6058ed-2673-4ff5-b1e6-4825cdf4183f&fileType=docx&objectUrl=https%3A%2F%2Fwaypointventures.sharepoint.com%2Fsites%2FMOACExamODMapping%2FShared%20Documents%2F1944%20AZ900%20Academifaction%20for%20EDU%2FAuthoring%20Guides%2FAuthor%20quick%20start%20guide_v2.docx&baseUrl=https%3A%2F%2Fwaypointventures.sharepoint.com%2Fsites%2FMOACExamODMapping&serviceName=teams&threadId=19:b9d59a11898a4a308177b4acb06ad4fe@thread.skype&groupId=829d72ca-0997-4a57-acbe-b86ad0097d72), and also [from GitHub](Author%20quick%20start%20guide.md).
- You *must* read the [Review the design doc guide](Review_the_design_doc_guide.md) before you begin authoring or reviewing content to familiarize yourself with the course's design, requirements and guidelines.

> **Note**: The Visio [GitHub Info graphic](https://teams.microsoft.com/l/file/02C384A9-D0C5-47ED-9E8A-416B451A333A?tenantId=4f6058ed-2673-4ff5-b1e6-4825cdf4183f&fileType=vsdx&objectUrl=https%3A%2F%2Fwaypointventures.sharepoint.com%2Fsites%2FMOACExamODMapping%2FShared%20Documents%2F1944%20AZ900%20Academifaction%20for%20EDU%2FDevelopment%20phase%2FGit%20Process%20flow%2FGitHubInfographic_v2.vsdx&baseUrl=https%3A%2F%2Fwaypointventures.sharepoint.com%2Fsites%2FMOACExamODMapping&serviceName=teams&threadId=19:b9d59a11898a4a308177b4acb06ad4fe@thread.skype&groupId=829d72ca-0997-4a57-acbe-b86ad0097d72) provides at a high level overview of the review process and workflow.

## Where to start
The following is the start point for all reviewers and will guide you to get up and running.

- Task 1: Ensure you have a clean local repo working environment
- Task 2: Create a branch in which to review in Visual Studio Code
- Task 3: Switch to your desired working branch in your local repo
- Task 4: Ensure you have the latest version of the repo
- Task 5: Start reviewing and editing the content
- Task 6: Modify or change image files in the content
- Task 7: Stage, commit and Push your changes up to the GitHub repo
- Task 8: Create a Pull request
- Task 9: Review the Pull request changes
- Task 10: Merge Pull request

### Appendices

The following supplementary [Appendices](Authoring%20guides%20source%20in%20markdown/appendices.md) provide more details and context.

- Appendix A: Components available for re-use from existing content
- Appendix B: An overview of basic Git terminology

> **Note**: A *test* repository \(repo\) is available from GitHub which mirrors the production repo. Use the test repo to try out Git actions *before* performing the actions in the production repo. Actions performed in the test repo are inconsequential. If you modify or delete your copy of the test repo, get a new copy at any time by using the **git clone** command in Visual Studio Code . Send an email to the team and we can re-create what you need from the test repo. The test repo is available at [https://github.com/WaypointVentures/Testrepo1](https://github.com/WaypointVentures/Testrepo1). If you do not have access to the test repo, email the team and request access.

### Task 1: Ensure you have a clean local repo working environment
The GitHub repository is available at [https://github.com/WaypointVentures/azfundedu](https://github.com/WaypointVentures/azfundedu). You may have already cloned this repo locally, however perhaps you have not worked in it in a while, or you made changes but can't remember what they were and are not sure you pushed them up, or are not sure in general what state your local repo is in, in relation to the GitHub repo. If you are unsure you should start with a clean local repo. This just ensures you have a clean repo to start your review and start work without worrying about making in advertent changes to the GitHub repo. You can do this as follows:

In this task, we will take a copy of our existing repo ad a backup, delete the existing repo, then do a new clone to ensure we have a clean state.

1) Go to the location where the local repo is stored in File explorer or some local file viewer. In the example below the repo is at `H:\DEVOPS\Repo\GitHub\waypoint`

    ![file explorer view with azfundedu repo folder and path highlighted.](images/review_cleanrepo_001.png)

    > Note: The folder name should be `azfundedu`, as this is the name of our production repo. If you look inside this folder you will see the folder structure that is present on GitHub. If you view hidden files you will also see a hidden `.git` folder which is used by editors to identify, manage and interact with the repo and GitHub    .

2) Create a folder alongside where the repo exists and call it `backup` and then a date or some way to differentiate between folders and any future copies you may make of the repo. You do not have to follow the naming convention exactly, this is just an example and suggestion.

    ![file explorer view with azfundedu repo folder and path highlighted.](images/review_cleanrepo_002.png)

3) Copy the entire `azfunedu` repo to the backup folder location you just created. The entire folder structure should be present within it.
    
    ![azfundedu copy.](images/review_cleanrepo_003.png)

4) Once the copy is complete delete the source `azfundedu` local repo folder which you copied

    ![azfunedu folder structure](images/review_cleanrepo_004.png)

> Note: If you get an error saying something like "Unable to delete.. Try Again.." it means a file from the repo is opened somewhere on your system. Close any editors, or files if they are open and any command line tools and then try again to delete the folder.

5) Once the folder is deleted, go to our GitHub repo [https://github.com/WaypointVentures/azfundedu](https://github.com/WaypointVentures/azfundedu) choose the `master` branch, and then click on the green `Clone or download` button and copy the URL by clicking on the copy icon beside the URL, as in the screenshot below.

    ![github repo clone or download url pane](images/review_cleanrepo_005.png)

6) Return to your local machine, open **Visual Studio Code** go to **View** > **Command Palette** and type `git clone` in the dialogue

    ![git clone command search.](images/review_cleanrepo_006.png)

7) Click on the `git clone` command that appears and in the resultant **Repository URL** dialogue, paste the GitHub URL we copied earlier from GitHub and press **Enter**.

    ![git clone command git url](images/review_cleanrepo_007.png)

8) A **Select Folder** window appears and in this select the location where you wish to place the product repo and click **Select Repository Location**. This could be where you originally had the repo, alongside the backup folder you created earlier. But it can be anywhere you wish. I would not recommend point to a remote storage location such as OneDrive, as folder and file name lengths can be long as a result and very long path names can cause problems, so keep the location local to your machine.

    ![select repository location dialogue](images/review_cleanrepo_008.png)

9) A status pane appears in the bottom left hand corner of visual studio code to inform you of progress and when finished it will prompt you to open the repo.


    ![git clone status prompt](images/review_cleanrepo_009.png)

    ![git clone open prompt.](images/review_cleanrepo_010.png)

10) Click **Open** and the repo will open in **Visual Studio Code** (VSC) on the master branch. If you do not want to open the repo now, you can do so subsequently in VSC by going to **File** > **Open Folder...** and the repo will display in folder view.


    ![git clone status prompt](images/review_cleanrepo_009.png)

    > Note: The repo and all its files and folders on GitHub are now present on your local machine. Your local repo is now an exact match of the repo on GitHub at this point in time, and you can be confident it is a clean state to start work in. 

### Task 2: Create a branch in which to review in Visual Studio Code
Each author will create a separate git branch for each module in which they will author. This separates content creation into its own working silo on a module by module basis and helps reduce the risk of any inadvertent changes to files. 

Reviewers will then create their own git branches off each author module branch, and perform their own reviews within that review branch. They can work in the content directly, make changes to markdown files as they need. Once their review is complete and all changes are staged and committed locally, then pushed to GitHub, a **Pull request** is opened on GitHub to merge the review branch back into the author branch. During that phase, authors can review the changes, and comments can be added by reviewers and authors about particular changes, and the edited files can be modified as needed once agreed between both. once final, the changes are merged into the author branch and the reviewer branch is deleted.

The author module branches will ultimately be merged back into the `master` branch, when complete also via Pull Request (PR), from which final docs will be published. 

You can create a branch in a number of ways, we will cover just one of those options here, namely **Visual Studio Code** (VSC)

> NOTE: We would recommend to do all the git tasks using Visual Studio Code. This may be the most straight forward and provide the most consistent environment to use. You are of course free to use any method that you prefer.

It is important that the review branch you are creating is based off the author branch for that module.

1) Ask the Author to confirm the name of the branch for the module you are about to review. You should receive a hand off email from the author and you should be clear on the following before you can proceed:

    - author name
    - module number ready for review
    - authoring branch name
    - files that are ready for review (or files that are not yet ready if that is the case.)
    - It should also be clear that the authors will not make any changes to their branches while the Review pass is underway. If changes are made in the author branch and review branch at the same time, that could result in merge conflicts, which we want to avoid. 


    > Note: The branch name authors use will be of the format \<mod number\>\<task\>\<author surname\>, all lowercase. For example

    - *author name* = **eamonn kelly**
    - *module author is working in* = **Module 5**
    - *resultant branch name*  = **m5authkelly**

    > This is really so the branch content and purpose is identifiable to anyone looking at the repo and that they know where to go to view certain content at various stages during the dev cycle. The name should be obvious what it contains. But again reviewers should confirm with the author before creating their review branch, to ensure they are looking at the correct content.

2) Also, again confirm which files are ready for review within that module branch with the author. There will be several outlines present in the module folder and not all may be ready for review at the same time.

3) Open **VSC** and go to **File** > **Open Folder**

    ![vsc windows with file > open folder highlighted.](images/git-vsc-createbranch-001.png)

4) Go to the location where you cloned the GitHub repo to your local environment and click **Select Folder**. The folder name you select for the production repo should be `azfundedu`

    ![open folder dialogue](images/git-vsc-createbranch-002.png)

5) The repo folder and file structure should now be visible in the explorer window in Visual Studio Code. Also present is a status bar at the bottom of the editor which tells you which branch you are currently on, **master** branch is listed in thi screenshot, 



    ![repo folder structure  vsc](images/git-vsc-createbranch-003.png)

    > Note: If you had the repo opened previously in VSC and did not close it i.e. just closed the app clicking the X or something,  it may be a different branch, so just be clear to check where you are working, as VSC will open up the last state it was in when previously opened.


6) Go to **View** > **Command Palette** and type git branch and in the resulaent set of commands click on **Git Create Branch From...**

    ![ list of branch names in branch pane](images/review_createbranch_001.png)

    > Important Note: There is another command available called `Git Create Branch`. Do not use this command, as this will base the branch you are about to create of whatever branch is listed in the status bas in VSC. Which in this case would be master. Ensure you select **Git Create Branch From...**

7) In the subsequent pane enter the name of the review branch you are creating and press **Enter** when done.

    > Note: The review branch name you use must be of the format \<mod number\>\<review type\>\<reviewer surname\>, all lowercase for example

    - *reviewer name* = **eamonn kelly**
    - *module am looking to start reviewing content in* = **Module 5**
    - *review am performing* = **technical review**
    - *resultant branch name*  = **m5techreviewkelly**

    ![ list of branch names in branch pane](images/review_createbranch_002.png)



8) In the subsequent pane from the list presented select the author branch you wish to base your branch off, in the screenshot we select `m5authekelly`

    ![ list of branch names in branch pane](images/review_createbranch_003.png)


    > NOTE: If you do not get a message prompting you for the branch on which to crate your new branch from, you may have selected the **Git Create Branch** command, and you should return to the earlier steps and ensure you select the **Git Create Branch From...** command


9) Your new branch should open up and the status bar should list that new branch as the branch in focus in VSC.

   ![ list of branch names in branch pane](images/review_createbranch_004.png)



    > NOTE: The newly created branch **only** exists in your local environment at this stage, as it has not been pushed up to GitHub. Nobody else can see or access the branch until it is pushed up to GitHub. As a last step before starting work you should now also push up that branch to GitHub so it is present there, as a back-up and also so other can view it as they need over time.


### Task 3: Switch to your desired working branch in your local repo
Your local repo may already be switched to the new branch depending on the steps you performed in earlier tasks. However, review these steps here to ensure you are in the correct branch. You will also have occasions where you will need to switch between branches in other scenarios apart from initial setup, and these steps will allow you to switch between branches.

Again, there are many ways to change branch, we will cover just using **Visual Studio Code**.


    > Note: You should commit, or delete, any unsaved file changes in an open branch before changing to a different branch. There are some details on this process and considerations [Stackoverflow - Git switch branch but keep modified files](https://stackoverflow.com/questions/35029866/git-switch-branch-but-keep-modified-files). If you have unsaved changes you will be prompted as such, and told that you will lose them if you change branches.


1) If you do not have a repo already open in VSC, open VSC and go to **File** > **Open Folder**

    ![vsc windows with file > open folder highlighted.](images/git-vsc-createbranch-001.png)

2) Go to the location where you cloned the GitHub repo to your local environment and click **Select Folder**. The folder name you select for the production repo should be `azfundedu`

    ![open folder dialogue(images/git-vsc-createbranch-002.png)

3) The repo folder and file structure should now be visible in the explorer window in Visual Studio Code. Also present is a status bar at the bottom of the editor which tells you which branch you are currently on, **master** branch is listed.

    ![repo folder structure  vsc](images/git-vsc-createbranch-003.png)

    > Important Note: If you are on a branch and then close VSC. When you reopen the repo, the same branch will be the focus. This will remain until you explicitly switch to a different branch.


4) Click on the branch listed in the status bar, in this case `master`, and in the branch pane that appears, note the list of all available branches in your repo, and select the one you wish to work in, in this case `m5authkelly` by clicking on it.


    ![vsc branch pane](images/git-vsc-createbranch-007.png)



5) The branch has now been switched to, and any changes made to these files are all done in this branch.

    ![vsc branch name in status bar](images/git-vsc-createbranch-008.png)


### Task 4: Ensure you have the latest version of the repo
One last action you should complete before you start authoring is to regularly ensure you have the latest version of the GitHub repo available in your local repo. Typically before you start working for the day, or if you need a particular file or feature that has just been added to GitHub that you don't have in your local repo.

There are two main methods for getting or synchronizing your local repo with GitHub, namely `git fetch` or `git pull`. git fetch will get the latest files from GitHub but will not merge the changes with your local repo, whereas `git pull` will get the latest files from GitHub and will merge the content with your local repo.

Other updates may have taken place in the GitHub repo by other contributors and you should ensure you always work in the latest version. Doing this can also help avoid merge conflicts which could arise should you make updates on content that has been updated previously by someone else, but you are working off an older version of the file.

However, you do still need to be careful that none of the changes have made locally are overwritten. Thus always make sure to stage and commit your changes to your local repo when finished working and do this regularly.See [Appendix B: An overview of basic Git terminology](Authoring%20guides%20source%20in%20markdown/appendices.md) for more details about git terminology and these actions if you need and have time.

If you have just performed the earlier tasks you may not have to do this, but there may arise occasions when it is needed, as such we include it here in case its needed.

1) Open **VSC** and the local repo as per the steps in **Tasks 1** and **2** earlier.

2) Change the branch to `master` as per the steps earlier in **Task 2a** and as indicated in the status bar in the screenshot below. 
    
    ![repo folder structure  vsc](images/git-vsc-createbranch-003.png)

3) Go to **View** > **Command palette**
    
    ![repo folder structure  vsc](images/git-vsc-createbranch-009.png)

4) Type **git** in the resultant pane tp view a list of all available git commands

    ![repo folder structure  vsc](images/git-vsc-createbranch-010.png)

5) Select the command `git pull` and the pull will commence. It will be indicated by spinning arrows in the status bar, beside the branch name. 

    > Note: You can also view the output of any commands you run by selecting **View** > **Output** and in the resultant output pane, select git form the drop down box

    ![repo folder structure  vsc](images/git-vsc-createbranch-011.png)


    > Note: You could also run a `git fetch` or any other git command available in VSC this way. Not all git commands are available in VSC. VSC does not have all git commands available in it. It just has a subset of common commands. It should be sufficient for what we are doing. If there is a scenario that's not covered you can always mail the team and we will investigate ad determine a solution.

    > Note: If there are committed changes in your local branch you may receive a message stating cannot overwrite existing changes, and you may need to resolve these conflicts in order to get the latest version. If there are un staged changes in your local repo, you may be prompted that you must commit these changes before you can complete the git pull. 



### Task 5: Start reviewing and editing the content
Markdown *outlines* are provided in the GitHub repo which can be used as starter files to help authors get up and running on each deliverable quickly. The markdown outlines provide the following, amongst other things:
- a framework within which authors can write the content needed for each file deliverable 
- an outline the various elements required in each file
- comments on how to author the various elements, guidelines, suggestions
- comments related to the markdown and if any particular formatting or structure is needed
- boilerplate text authors you can re-use  

Reviewers are able to make changes directly in the authors markdown files. Reviewers do not need to log items in an xls file, or add additional comments to the content markdown. You can if you wish, but it is not necessary. Authors will review the changes reviewers make in the .md files, through a Pull Request (PR) on GitHub, once you are finished your review and it has been pushed up to GitHub. Authors will review the changes side by side, comparing the author branch to the reviewer branch, and they can add comments, and edit the files as they agree or disagree with any changes, all in GitHub via a web browser. 


The next step is to choose the correct outline in which to get started

1) Open your markdown editor, namely **Visual Studio Code**, and go to **File** > **Open Folder...** > open the folder containing our production repo.


    ![git gui Merge > Local merge menu](images/vsc_files_001.png)

2) Go to the Module that you wish to start are reviewing for i.e. `Course Materials\Modules\Mod0X`, where `X` is the module number you wish to work on,  and then choose the outline file that you wish to start in. In this case we open `40574A Azure Fundamentals Module 1 Student Guide.md`

    ![git gui Merge > Local merge menu](images/vsc_files_002.png)

    > **NOTE**: All the files listed under each Module folder are outline markdown files, which help authors start on the content development. Choose whichever one you wish to start working in first. These files [Here](https://github.com/WaypointVentures/azfundedu/tree/master/Author%20templates%20and%20outlines/Final/md)

    > NOTE: A full list of the deliverables and outlines is available in the BOM in Teams. If you have queries around that you can raise those with the project manager.

    At the time of writing there are 8 outlines available, listed below but this will continue to grow and you may see different files also present

    - `40574A Azure Fundamentals Module X Lesson X Topic X Learning Activity Support Starter.md`
    - `40574A Azure Fundamentals Module X Lesson X Topic X Learning Activity Teach Starter.md`
    - `40574A Azure Fundamentals Module X Lesson X Topic X Learning Activity Try it Starter.md`
    - `40574A Azure Fundamentals Module X Supplemental assessment questions.md`
    - `40574A Azure Fundamentals Module X Student Guide.md`
    - `40574A Azure Fundamentals Module X Module Preparation Guide.md`
    - `40574A Azure Fundamentals Module X Cornerstone Lesson Plan.md`
    - `40574A Azure Fundamentals Module X Lesson Plan 1.md`


3) Reviewers can make changes directly in the markdown. As you make changes to the markdown you can view how the changes will display by viewing the file in **Preview** in **Visual Studio Code**. You can access this by clicking the **Preview** button in the top right hand side. This allows you to see how the file renders in real-time.
    
    ![.md tab open and Preview button highlighted](images/vsc_files_003.png)

    ![vsc .md and preview tabs open](images/vsc_files_004.png)

4) You can now start reviewing and making changes to the outline file as needed. You can re-use the source elements to help you create that content if you need.

    > NOTE: Ensure you save the file regularly while working so as not to lose any work. There is auto save functionality in Visual Studio Code, which is available by going to **Settings** > **Commonly Used** > **Auto save** and setting the desired function. i.e. perhaps `afterDelay` and then a value in milliseconds.

    > NOTE: Ensure you `stage`, `commit` and `push` your work regularly as well. small regularly commits are preferred to one big `stage`, `commit` and `push` at the end.


### Task 6: Modify or change image files in the content
This may or may not be relevant to your review. You can modify or update graphics to the markdown file as follows if you need to.

1) Create whatever screenshot or graphic you want to include in your content, and save it in .png format. You can use other formats, but we will adhere to .png to standardize the files.

2) Once you have the graphic created you need to copy the graphic to the following location in your local repo, depending on your module number i.e. `Course Materials\Modules\Mod 0X\media`. It does not need to be on GitHub at this stage, just your local repo, in which you are working.

    > Each module has its own **media** folder that sits alongside the outlines. All graphics should be placed inside the media folder within the module you are working.

    ![file explorer media folder](images/media_001.png)

    > Note: There is a media folder outside of the Module folders, immediately under **Course Materials**. This is for use for non-module specific files.

3) Return to the markdown file where you want your image to display and enter the below

    ```bash
    ![enter alt text](media/image_name_001.png)
    ```

    > Note: The **alt text** is a description of the image for use by the visually impaired. It appears in the published doc, and is a legal requirement for accessibility. So it must be added for all images.
    
    > Note: You should also name you images with some identifiers, namely, `<module number><descriptor><number value defined by three digits>.png`. i.e. `mod01_azureportal_001.png`. Currently all images are divided out per module in their own media folder, but this could change, so use of good naming conventions will help identify you module images if needed.

    > Note: The path to the image must be as the path listed above i.e. `media/imagename.png` 

    > Note: You can also indent the graphic line in markdown to be in line with numbered steps etc. Typically it should be on its own line aligned to the left side, but you can indent the image line if you need.

4) Verify your newly added image is displaying as you intended in your markdown file by using the **Preview** feature in Visual Studio Code. this just helps to ensure there is no typos, incorrect indentation causing the image to not display, or not display as intended.

    ![file explorer media folder](images/media_002.png)
    
    > NOTE: If you need to change a graphic you do not need to modify the markdown content. You can just create the image and overwrite the existing graphic in the media folder.
    
    > Note: There are also images available from the Source content in the GitHub repo. These are present at `AZ900-AzFund\Modules\Linked_Image_Files` and you can check the individual source content markdown files for the image names called in each topic. Details of the source content markdown files that are available per lesson, are outlined in the Design doc on the teams site.



### Task 7: Stage, commit and Push your changes up to the GitHub repo
You should periodically stage and commit any work to your local repo, and then push your changes to the GitHub. This is to back up your work and also to make it visible it other as they need. It also help us keep the work being done granular, and in small commits, rather than one large commit at the end. This is helpful when we go to merge the changes into the author branch via Pull Request.

There are three stages to adding files to the GitHub repo

1) **Staging**: This gets the updated or new files ready to be committed to the local git repo.
2) **Committing**: This commits the staged changes to the local repo. 
3) **Pushing**: This pushes the changes from the local repo to the GitHub repo.

You can do these steps a number of ways but we are just doing them in **Visual Studio Code (VSC)**


1) If you have made changes in any of the files you need to save them. You can do this by pressing **Ctrl+S** or **File** > **Save** in **VSC**.

    Any updated file is now saved locally in our file system, but we have not staged or committed it yet to our local repo or pushed up to GitHub.

2) Go to our GitHub repo and verify the branch or file is not present. This is just so we can validate the change after we push the update. You do not need to do this step all the time, just when getting familiar with the process and commands, to build trust.

    ![GitHu repo file not present](images/vsc_push_005.png)


3) In **VSC** go to **View** > **Output**. This will open up the output area in the bottom right hand area of the VSC window.

    ![Visual Studio Code View > Output...](images/vsc_push_001a.png)

    > **Note**: This is not essential to be able to stage, commit and push updates to repos. It is done here just to allow you to view the commands and output as they run, if you want to see what's going on underneath the hood.

4) Again in **VSC** with the repo folder open, go to **View** > **Command Palette...** 

    ![Visual Studio Code View > Command pallette...](images/vsc_push_001.png)

5) In the **Command Palette** window, type **git**. The available git commands will display

    ![vsc Command pallette git commands displayed](images/vsc_push_002.png)

6) Select the command **Git: Stage All Changes**

    ![vsc git stage all changes command highlighted](images/vsc_push_003.png)

7) You may receive a prompt to **Choose a repository**, select the repo you are working in by clicking on it. 

    ![vsc choose a repository](images/vsc_push_004.png)

    > Note: You will see the git command execute in the **Output** pane as the command is run.

8) In VSC under **Open Editors**, hover the mouse over the file and you will see the file now has the detail of **Index added** to it, it did not have this previously.

    ![vsc choose a repository](images/vsc_push_006.png)

9) Open the **Command Palette**,  type **git** and select the command **git: Commit** . This will commit the staged update to the local repo. 

    ![vsc command pallet git commit command highlighted](images/vsc_push_007.png)

10) Again, you may receive a prompt to **Choose a repository**, select the repo you are working in by clicking on it. 

    ![vsc choose a repository](images/vsc_push_008.png)

    > Note: You will see the git command execute in the **Output** pane as the command is run.

11) You will be prompted to enter a message for the commit. this should be a description of the change being made sop other can understand what the change is. This description will be visible in a number of places such as logs and on the GitHub repo alongside the file itself.

    ![vsc command pallet git push command highlighted](images/vsc_push_008a.png)

12) Once the command is finished the index added association with the change will now be gone.

13) Open the **Command Palette**,  type **git** and select the command **git: Push** . This will push the committed changed to the GitHub repo. 

    ![vsc command pallet git push command highlighted](images/vsc_push_009.png)


14) Again, you may receive a prompt to **Choose a repository**, select the repo you are working in by clicking on it. 

    ![vsc choose a repository](images/vsc_push_010a.png)

    > Note: The icons associated with the repo change to arrows, indicating it has been committed locally and is ready to be pushed up to the GitHub repo. The icon was a plus sign during the staging process. You will see the git command execute in the **Output** pane as the command is run. When it is complete you can. You will also see spinning arrows in the status bar. When these stop spinning the command has completed.

15) When the command is complete, go to GitHub repo and verify the updates are present in GitHub. 


    ![vsc choose a repository](images/vsc_push_012.png)

    > Note: If they are not present, you should check that you successfully staged and committed the updates, and repeat those actions again to verify.


16) If you receive an error saying **Can't push refs to remote. Try running `pull` first...**. You will need to perform a `git pull` on the GitHub repo to get the latest version of the GitHub repo to your local repo. Once this is complete, you should try perform the `git push` again.

    ![vsc git push error](images/vsc_push_011.png)


17) If you receive a message saying a branch has no upstream branch, it means the branch is local only and does nto exist on GitHub. As such it is asking do you wish to publish the branch to GitHub. If you click Yes, it will make the branch available on GitHub. 

    ![vsc git push error](images/review_push_publishbranch_001.png)

17) If you receive a message saying "... permission denied..." This is most likely because a file in the repo is open somewhere on your system. Ensure all files closed and try again.


### Task 8: Create a Pull request
When you are finished your review and you have staged, committed and pushed all changes to GitHub we need to start the process of review and merging with the author content. We do this using Pull Requests (PRs). If you wish to read more about Pull Requests you can start on the page [About Pull requests](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests). I would recommend you read some information here to try get familiar with the concepts and test it out on the Test repo if you have time.

1) At this stage Waypoint will create the pull request for the reviewer and author. You can initiate this process by emailing the Waypoint team including the author, asking for the creation of a pull request including the following information in the mail:

    - Module number
    - Review type (i.e. ID, copy edit etc.)
    - Review branch name
    - Author branch name

    > NOTE: The following steps are provided as information, reviewers are not expected to complete them, however they should read through them as they may be useful to gain an understanding of the process.

2) The Pull request will be created in GitHub by going to the production repo, [https://github.com/WaypointVentures/azfundedu](https://github.com/WaypointVentures/azfundedu), on GitHub and selecting **Pull requests**

    ![vsc git push error](images/review_prcreate_001.png)

3) Click **New pull request**

    ![vsc git push error](images/review_prcreate_002.png)

4) On the **Compare changes** pane select two items 

    - Left button > the `parent` or `base` branch on the left, this would be the author branch into which we are merging changes.  
    - Right button> the `child` branch which contains the updates we wish to merge i.e. the reviewers branch.

    ![vsc git push error](images/review_prcreate_003.png)

    > NOTE: We can see a preview list of changes that will be made as part of the Pull request already, underneath the branch selection buttons, and we can scroll down, open and review the changes before creating the Pull Request.

5) Click the **Create pull request** button to create the Pull request

   ![vsc git push error](images/review_prcreate_004.png)

6) Enter a title and some descriptive text explaining what the PR is for i.e. `Mod 5 ID review branch merge with author branch` or something like that, then click **Create pull request**

   ![vsc git push error](images/review_prcreate_005.png)

    > NOTE: The pull request name should be in a format something like the following \<module number\>\<review type\>\<review branch name\>\<author branch name\>. As with branch names, it should be obvious for anyone looking at it what it is doing.

7) The Pull request has now been created and is visible to everyone on GitHub by going to the pull request tab and selecting the pull request in question, as in the screenshot. 

   ![vsc git push error](images/review_prcreate_006.png)

    > Note: There may be multiple PRs open at the same time.

### Task 9: Review the Pull request changes 
Authors must first review the changes in the PR and decide if they agree with them or not.

**General Functionality of PRs**:
- Provides a diff of the changes between the two branches which is displayed and visible in GitHub via web browser, red indicates deletions, green indicates additions.
- There is no way to accept or reject individual changes in a PR,
- Where an author disagrees with a change It is possible to edit files directly, in GitHub in a web browser, and make the changes an author wishes to see.
- It is possible to add comments, and have a discussion in the PR between author and reviewer in the PR via a web browser to clarify if a change is needed or not.
- Where an author agrees with a change they do nothing, this indicates acceptance of the change.

The first step is for the author to review the changes

1) Go to GitHub and open the PR that has been created, and click on the **Files changed** tab

    ![vsc git push error](images/review_prcreate_007.png)

2) Within this tab it is possible to see all the changes that have been made. You can click the arrow on the left hand side beside the filename to expand or collapse the file in question and view the changes or not. Items being replaced, or deletions are visible in `red`, items being added are highlighted in `green`.


    ![vsc git push error](images/review_prreview_002.png)

    ![vsc git push error](images/review_prreview_001.png)


3) Add a comment to a change, or specific area of the file if you need to query a specific change, or wish to have a discussion on a particular point, by hovering your mouse over a part of the file on display and clicking the `blue box with white plus sign`, enter your comment and click **Start a review**. You can preview your comment also by clicking the preview tab.

    ![vsc git push error](images/review_prreview_004.png)

4) This creates a `review` which the reviewer can then see and reply to in the same comment area by typing text into the reply box. In this way a conversation can be had about specific points in GitHub in your web browser. You may have to support or supplement with email where deeper discussion is needed, but the GitHub review comments can initiate that, and form the basis of that process.

    ![vsc git push error](images/review_prreview_005.png)

    ![vsc git push error](images/review_prreview_006.png)

    > NOTE: You can return and edit already posted comments if you wish as well.


5) Edit a file by clicking on the three dots on the right hand side of the file in question

    ![vsc git push error](images/review_prreview_007.png)

6) An in-browser editor opens and you can make any changes you need by typing directly in the browser editor. You can preview those changes in the browser also. The full file is available and you can scroll down through the file in question.

    ![vsc git push error](images/review_prreview_008.png)

7) When complete, scroll down to the end of that editor page, enter a short title and description, ensure commit directly to the review branch is selected, and click **Commit changes**. 

    ![vsc git push error](images/review_prreview_009.png)

8) The change you just made is now visible in the file as part of the pull request.

    ![vsc git push error](images/review_prreview_010.png)

9) Other functionality that is available within PRs is the ability to click the **Viewed** checkbox. Authors should click the checkbox as **Viewed**, when they have completed their review of a file and they are happy with all the changes. This just provides an indication that a file is finished and good to go. Status of the files review is then visible to all on that PR page.

    ![vsc git push error](images/review_prreview_011.png)


10) There is also an option to display a rich diff, which will show a Preview version of the file changes, similar to a Track Changes option in word. If you need you can click the Display the rich diff button to view this pseudo track changes version

    ![vsc git push error](images/review_prreview_012.png)

11) You can return to the default diff view by clicking the **Display the source diff** button

    ![vsc git push error](images/review_prreview_013.png)

12) It is also possible for 3rd parties, i.e. not the author or reviewer to review and approve the changes, or add comments and opinions to the changes and engage in the review process. You can do this by clicking on the **Conversation** tab entering the comment and submitting the comment. There are also emoji's available to use, if you wish, and you can have conversations within here and ultimately be able to agree and resolve a discussion point or conversation.

    ![vsc git push error](images/review_prreview_014.png)


13) Continue through the review process and engagement between the reviewer and author until all changes are agree between both parties.


### Task 10: Merge Pull request
When all file changes have been agreed and the files are final we need to then merge the changes into the author branch. This will be done by the waypoint team. 

1) When all files are final send an email to the waypoint team and state the following

- module number
- review type
- Pull request number
- reviewer branch name
- author branch name
- state that all flies have been reviewed, all changes have been implemented and the files are now final and ready to be merged into the author branch.

2) The waypoint team will then open up the pull request and on the **Conversation** tab, go to the green **Merge pull request** button and select the **Create a merge commit** option.

    ![vsc git push error](images/review_prreview_015.png)

3) The click on the **Confirm merge** button

    ![vsc git push error](images/review_prreview_016.png)

4) You will receive a message stating the branch has been successfully merged, and you can then click on the subsequent **Delete branch** button

    ![vsc git push error](images/review_prreview_017.png)

5) You can then view your changes in the files by clicking the **Code** tab in the repo and going to the files in question in the author branch. Verify the changes are now present in the author branch as expected.

    ![vsc git push error](images/review_prreview_017.png)

    > Note: You have now successfully reviewed and merged updated content into the author branch.
