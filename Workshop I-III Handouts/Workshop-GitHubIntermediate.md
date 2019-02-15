## Workshop II: GitHub for Intermediate Users

# The Plan

1. Working with the GitHub Desktop Client
   * Cloning a repo
   * Branches, Commits, and Pull Requests
   * Working with a forked repository
2. Resolving merge conflicts

## The GitHub Desktop Client  

You can accomplish quite a bit working in the web version of GitHub, but sometimes you need to work locally rather than in an online environment.  Installing the GitHub desktop client gives you more flexibility in how you can interact with the documents and files within our repository.

Download GitHub Desktop (available for MAC and PC), [https://desktop.github.com/](https://desktop.github.com/).  

### Setting up GitHub Desktop  

Add your GitHub.com account information to GitHub Desktop to access your repositories. Open GitHub Desktop and click on **Options** in the file menu

![Imgur](https://i.imgur.com/5oXCqd9.png)

In the **Accounts** tab, sign in to your GitHub.com account.  You can also opt to sign in via your browser. If you have two-factor authentication enabled, you will be prompted to authenticate.

![Imgur](https://i.imgur.com/xnlewp0.png)

Next, click on the **Git** tab to add your email address.  GitHub Desktop will use the email address you set in your local Git configuration to connect Commits with your GitHub account.  Locate your email address in GitHub by going to account settings and clicking on **Email**. *Note: I prefer to kept my email private and use a no-reply email address supplied by GitHub*.

![Imgur](https://i.imgur.com/dwRoIOQ.png)

Lastly, in the **Advanced** tab, select your external text editor.  We recommend installing Atom, [https://atom.io/](https://atom.io/), an open source text editor with Git and GitHub integration built in.

![Imgur](https://i.imgur.com/pkEIhQ8.png)

## Cloning Your Repository  

During the last session, we created a repository called **Hello-World**.  Let's clone Hello-World to our GitHub Desktop.  You can clone a repository from GitHub Desktop or from the repository's main page on GitHub.

### Cloning a Repository from GitHub Desktop  

In GitHub Desktop, click on **File** and select **Clone repository**.

![Imgur](https://i.imgur.com/vXA7gNI.png)

This will open a dialog box where you have two options.  
1. From the **GitHub.com** tab
  * Select your repository from the available list and click Clone. *Note the local path; this is where your files will be stored on your computer*
2. From the **URL** tab
  * Paste/ type in the repository URL OR your GitHub username and repository. *Note the local path; this is where your files will be stored on your computer*

![Imgur](https://i.imgur.com/L7fFCTI.png)

### Cloning a Repository from GitHub  

Go to the main page of your repository on GitHub and click on the green **Clone or download** button; select **Open in Desktop**

![Imgur](https://i.imgur.com/ExjFHVz.png)

### Care and Feeding of Your Cloned Repository  

After successfully cloning your repository, you will have two copies: 1) the local copy on your computer, and 2) your repository on GitHub (a.k.a **remote** or **origin**). Keeping these two copies in sync will be an important part of your workflow!

Why is syncing so important?  
1. Ensures that you are always working with an up to date repository.
2. Helps you avoid merge conflicts

When you open your repository in GitHub Desktop, it will automatically pull the latest version of your GitHub repository (**fetch origin**).  You can manually sync by clicking on the **fetch origin** button or by clicking on **Repository** and selecting **Pull**.

![Imgur](https://i.imgur.com/SbAty81.png?1)

When you're done working locally and have commits to push to your GitHub repository, the **Fetch origin** button will change to **Push origin**.  You can either click on the button or click on **Repository** and select **Push** to push your commits to your repository.

![Imgur](https://i.imgur.com/Y5XxN5M.png)

## Working with Branches in GitHub Desktop  

Creating a **branch** in your repository allows you to isolate development (developing new features, fixing bugs, experimenting with new ideas...) without impacting your entire repository.  Each repository has one default branch, **master**, and you can create as many other branches as you need.

##### To Branch or Not to Branch:
* Scenario:  Working with simple text files or making a minor edit - Live dangerously and work in your master branch  
* Scenario: Testing out a new idea - Create a branch  
* Scenario: Doing some heavy duty development on features - Create a branch  
* Scenario: Developing a GitHub Pages site for your repository - Create a branch  
* Scenario: Working with a group of collaborators - Create a branch  
* Scenario: If your changes have the potential to blow up your repository - Create a branch!

Let's create a branch in our cloned repository, Hello-World. Click on **Branch** and select **New branch**.  Give your branch a name and click **Create branch**.

![Imgur](https://i.imgur.com/Y8aLS5P.png)

Publish your branch to GitHub which will allow you to share it, open a pull request, and collaborate with others.

![Imgur](https://i.imgur.com/jcNuJpf.png)

Switch between branches by clicking on the **Current branch** button.  Remember, **master** is your default or production branch.

![Imgur](https://i.imgur.com/N97pQw7.png)

Working in the new branch we just created, let's make an edit to one of the files in our Hello-World repository.  Commit the change to the new branch you created.

Compare your new branch with the master branch by clicking **Branch** and selecting **Compare to branch**. The new branch is one commit ahead of the master.

![Imgur](https://i.imgur.com/Bk0ctkg.png)

To merge your changes into the master branch, switch the current branch to master, click on **Branch** and select **Merge into current branch**. Select the new branch in the dialog box and click on the merge button below.

![Imgur](https://i.imgur.com/OIbpWMY.png)

Now that the branch has served its purpose, delete it by clicking on **Branch** and selecting **Delete**

![Imgur](https://i.imgur.com/sEaq6ZF.png)

##### *If you are working collaboratively, best practice is to create a pull request before merging in changes.*


## Working with a Forked Repository

Building your own repository can be fun, but sometimes you just want to contribute to an existing project or maybe you'd like to use someone else's project as the starting point for a new project of your own. If that's the case it's time to **Fork**.

Creating a **fork** creates a personal copy of someone else's project. You can contribute back to the original project by submitting Pull Requests.

We're going to create a fork of the **Learning-GitHub** repository created by **HeardLibrary**.

* Navigate to the main page for the **Learning-GitHub** repository in GitHub; you cannot fork a repository from GitHub Desktop. Click the **Fork** button in the header of the repository. This will create an exact duplicate of HeardLibrary's Learning-GitHub repository under your own GitHub username.

![Imgur](http://i.imgur.com/Bi0jTS8.png)

Currently your fork of the Learning-GitHub repository only exists in the GitHub web client, but we need to clone it to your computer.

* Navigate to your fork of the Learning-GitHub repository.  Click on the green **Clone or download** button on the right side of the screen and click open in desktop.

![Clone repository](https://i.imgur.com/bmtSa3P.png)

* Once you've successfully cloned the repository, all the repository files will be available to you on your desktop.  Let's make some changes to the _**TakeAways.md**_ file.
  * Commit your changes and then click on the **Push origin** button to push your changes from the desktop client to your forked repository on GitHub.com.

To contribute these changes back to the original repository, you'll need to create a pull request.  We'll take a deep dive into pull requests in the third workshop.

## Working with Merge conflicts  


## GitHub Tutorials and Resources:
**GitHub Desktop Guides** [https://help.github.com/desktop/guides/](https://help.github.com/desktop/guides/)
**GitHub Guides** [https://guides.github.com/](https://guides.github.com/)
**GitHub Training & Guides** [https://www.youtube.com/user/GitHubGuides/featured](https://www.youtube.com/user/GitHubGuides/featured)
**GitHub Help** [https://help.github.com/](https://help.github.com/)
