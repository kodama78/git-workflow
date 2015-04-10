# Web-1

This reposiotry (**repo**) was built to run through a step by step process to understand the Github task workflow we utlize at [LearningFuze](http://learningfuze.com). We will be using the following tools:
- Git using Terminal (Mac) or GitBash (Windows) - [Download](http://git-scm.com/downloads)
- Github.com
- SublimeText 3 Text Editor - [Download](http://www.sublimetext.com/3)

The workflow outlined in the readme below will be utilized for every assignment/task/project for the course so understanding how and why is super important. If you have any questions please feel free to email instructors@learningfuze.com


## Assumptions we are making
- You have Git installed on your system, [how do I know if git is installed?](http://lmgtfy.com/?q=how+do+i+know+if+git+is+installed+on+my+computer)
- You have read these Guides
	- [Why Git & Github](https://docs.google.com/document/d/1Kyrj_xEXGja4R_-syhBuoYLo53urUIL_YDNEi56Qi9w/pub)
	- [First Github Project](https://guides.github.com/activities/hello-world/)
	- [Understanding Github Flow](https://guides.github.com/introduction/flow/)
	- [Forking Projects](https://guides.github.com/activities/forking/)

## Getting the files locally

### Step 1 - Forking the Repo
- Fork this repo by clicking the "Fork" button located on the top right of this page
	![Fork Button](https://github.com/ej020586/web-1/blob/assets/assets/fork.jpg?raw=true)

### Step 2 - Opening Command Line & navigating to your sandbox
- Open up command line tool Mac(Terminal), PC (Git Bash) in your sandbox folder. [Where is my sandbox Folder?](https://docs.google.com/document/d/1GYqDtY12-RgzrbbHzY7kqxpqP_y_X6c5sNKH9NLqMPM/pub)
		
	**Mac EASY**
	- If you have not done so already, enable [Easy osx terminal window opening](https://github.com/ej020586/web-1/blob/osx_easy_terminal/osx_easy_terminal.md)
	- Go to a folder in your finder 
		- ![Folder](https://github.com/ej020586/web-1/blob/osx_easy_terminal/assets/folder.png) - - 
	- Right click on the folder and look for *"Services"* at the bottom (sometimes it glitches and you will need to do this twice)
		- ![Folder](https://github.com/ej020586/web-1/blob/osx_easy_terminal/assets/services.png) - - 
	- Select the option *"New Terminal Tab at Folder"* 
		- ![New Terminal At Folder](https://github.com/ej020586/web-1/blob/osx_easy_terminal/assets/new_terminal_tab.png) - - 
	**Mac not-so-easy**
	- Press the command key and space bar
		- You should see the spotlight search appear
		- type in Terminal and hit enter
	- Type in `cd ` (which stands for change directory) then drag your folder into the terminal window
	- For a computer user of "test" the line would look like this
		- `cd /Users/test/Desktop/sandbox`
		- *You should see "test" replaced with your computer username*
	- Hit Enter

	**PC**
	- Open windows explorer to the sandbox folder
	- Right click and select "Git Bash Here" shown in the image below
	![Shortcut Git Bash](https://lostechies.com/jasonmeridth/files/2011/03/image_thumb_70716233.png)

### Step 3 - Cloning the repo
- Type in the following into your command line 
	- `git clone https://github.com/ej020586/web-1.git` and hit enter
		- The **clone** command tells git to copy the contents of the master branch
		- *The url after the word "clone" can be found in the right hand side panel of this page under the Settings link. You can click the button to the right of the url that will automatically copy this url for you*
- Then type `cd web-1` and hit enter

#### Congratulations you have cloned your first Github Repository

## Editing your files

### Step 1 - Opening your web-1 directory

- Start SublimeText Editor
- Open web-1 directory by clicking on File->Open
	- Select the web-1 folder under the sandbox folder on your desktop
	![Open Image](https://github.com/ej020586/web-1/blob/assets/assets/open.jpg?raw=true)

### Step 2 - Add basic HTML
- Open the index.html file by clicking on the file name on the left hand side in SublimeText
- Add html, head, body tags to the index.html file
- Add a h1 tag with the text "Hello World" inside the tag
- Add a p tag with the text "This is my first web page"
- Save the file by selecting File->Save

### Step 3 - View in the browser
- Navigate to the web-1 folder
- Right click on the index.html file and select open with Chrome
![Web Page](https://github.com/ej020586/web-1/blob/assets/assets/web-page.jpg?raw=true)

#### You have done it! The basics of creating your first web page

# Now What?
You may think that we are done there is nothing left to do because the task is complete but my question is. How does your Manager or Instructor know that you have completed the task Outlined for you? The answer is they don't. You only have the files locally and there for everyone else is left in the dark. We don't know if you have completed the task, we don't know if you have had any issues with the task.

### How do we address this?
We address the issue by allowing others to see our work through a centeralized Repo (Github.com).

### How do we get our files to Github?

The quick answer is by doing these steps within your command line tool

1. `git add .` - Add all files
2. `git commit -m "message describing what i'm commiting"` - Commit the files that were added (staged)
3. `git push origin master` - Push these files to a remote location (origin master)

### What do these lines mean?

#### Step 1 - git add .
- `git add` is the command we use to stage files for a commit. This tells the `git commit` command which files we are saving together
- The **.** part of the command is used to tell git we want to add **all** files that have been changed or modified.

#### Step 2 - git commit -m "message describing what i'm commiting"
- `git commit` is the command we use to commit that staged files to our local repo
- **-m** tells our commit command we want to add a message
- The text that is surounded by quotes is the message we want to add with our commit.
- *A good commit message describe the functionality that was changed* The files that were added/edited/deleted will be easy to find within the commit

#### Step 3 - git push origin master
- `git push` is the command that takes our local repo and pushes the commits to a remote location
- **origin** describes the remote location. More about git remotes [here](http://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes)
- **master** describes the branch you are pushing too. More about branching later but for now pushing to master will be the default

##### [Cheat Sheet](https://training.github.com/kit/downloads/github-git-cheat-sheet.pdf)

### After pushing your local branch you will see the changes on Github under your repository


