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

![Imgur](https://i.imgur.com/L7fFCTI.png)


## Working with a Forked Repository

Building your own repository can be fun, but sometimes you just want to contribute to an existing project or maybe you'd like to use someone else's project as the starting point for a new project of your own. If that's the case it's time to **Fork**.

Creating a **fork** creates a personal copy of someone else's project. You can submit Pull Requests to help make other people's projects better by offering your changes up to the original project. We're going to create a fork of the **Learning-GitHub** repository created by **HeardLibrary**.

* Navigate to the page for the **Learning-GitHub** repository, and click the **Fork** button in the header of the repository. This will create an exact duplicate of HeardLibrary's Learning-GitHub repository under your own GitHub username.

![Imgur](http://i.imgur.com/Bi0jTS8.png)

Currently your fork of the Learning-GitHub repository only exists in the GitHub web client, but we need to clone it to your computer.

* Navigate to your fork of the Learning-GitHub repository.  Click on the green **Clone or download** button on the right side of the screen and click open in desktop.

![Clone repository](https://i.imgur.com/bmtSa3P.png)

* Once you've successfully cloned the repository, all the repository files will be available to you on your desktop.  Let's open a text editor (Use Notepad today, but I recommend installing ATOM, [https://atom.io/](https://atom.io/), for your personal use) and make some changes to the _**TakeAways.md**_ file.
  * Remember to create a working branch first!
  * Commit your changes and then click on the **Sync** button to push your changes from the desktop client to GitHub.com.

* Now it's time to propose changes into the main project.
  * Go to your fork of the repository on GitHub.com and click on the green **Compare & pull request** button or use the pull request tab to create your pull request.

![Imgur](https://i.imgur.com/QbV4Dci.png)

Once the pull request is submitted, it is up to the project owner whether your changes will be pulled into the repository or not.

### For more tutorials and resources about using GitHub visit:
**GitHub Guides** [https://guides.github.com/](https://guides.github.com/)
**GitHub Training & Guides** [https://www.youtube.com/user/GitHubGuides/featured](https://www.youtube.com/user/GitHubGuides/featured)
**GitHub Help** [https://help.github.com/](https://help.github.com/)
