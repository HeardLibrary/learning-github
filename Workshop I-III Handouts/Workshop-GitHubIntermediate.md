## Workshop II: GitHub for Intermediate Users

# The Plan

1. Working with the GitHub Desktop Client
   * Cloning a repo
   * Branches, Commits, and Pull Requests
   * Working with a forked repository
2. Resolving merge conflicts

## Working with a Forked Repository

Building your own repository can be fun, but sometimes you just want to contribute to an existing project or maybe you'd like to use someone else's project as the starting point for a new project of your own. If that's the case it's time to **Fork**.

![Forking a repository](images/forks.jpg)

Creating a **fork** creates a personal copy of someone else's project. You can submit Pull Requests to help make other people's projects better by offering your changes up to the original project. We're going to create a fork of the **Learning-GitHub** repository created by **HeardLibrary**.

* Navigate to the page for the **Learning-GitHub** repository, and click the **Fork** button in the header of the repository. This will create an exact duplicate of HeardLibrary's Learning-GitHub repository under your own GitHub username.

![Imgur](http://i.imgur.com/Bi0jTS8.png)

We've been able to make edits to our files in the web version of GitHub, but that can get tricky.  Installing the GitHub desktop client gives us more flexibility in how we can interact with the documents and files within our repository.

Download GitHub Desktop (available for MAC and PC), and login to your GitHub account in the desktop client.  [https://desktop.github.com/](https://desktop.github.com/)

Now that you've successfully installed GitHub Desktop and forked the Learning-GitHub repository, it's time to get to work.  Currently your fork of the Learning-GitHub repository only exists in the GitHub web client, but we need to clone it to your computer.

* Navigate to your fork of the Learning-GitHub repository.  Click on the green **Clone or download** button on the right side of the screen and click open in desktop.

![Clone repository](https://i.imgur.com/bmtSa3P.png)

* Once you've successfully cloned the repository, all the repository files will be available to you on your desktop.  

## Cloning a repository using the desktop client

In addition to cloning a repository from the website side, you can also clone from your local computer using the GitHub desktop client.  The process described here will work for cloning one of your own repositories, a repository that you've forked to your account from elsewhere, or another repository that you don't own, but to which you have been given write access.

Drop down the Current Repository menu in the upper left of the window.  Click on the Add dropdown and select "Clone Repository...".

![Select clone option](images/desktop-clone-option.png)

You'll be presented with a list of repositories at Github.com to which you have access.  Repos that you own or to which you have write access will show up with little book icons.  Repos that are clones of some other repo will have a little "fork" symbol.  Click on the name of the repo you want to clone and you'll have an opportunity to select where you want the local copy of the repo to live on your computer.  Once you've selected a location, the desktop client will default to that location the next time you clone.

![Select clone location](images/desktop-clone-location.png)

![Cloning process](images/clone.jpg)

## Working with cloned files

After you've finished the cloning process, in the left column of the client, you'll see either changed files or the commit history, depending on which tab you've selected.  

![Changed files](images/desktop-changed-files.png)

By dropping down the Current Repository list, you can switch to a different cloned repository, including one that you cloned from the GitHub website side. By default, the desktop client chooses the master branch of a newly cloned repo.  However, you can change from the master branch to another existing branch by dropping down the middle "Current Branch" menu at the top of the window.  

![Current branch](images/current-branch.png)

When you select a default branch in this dialog, we say that your are "checking out" that branch. Checking out a branch literally changes the files that are present on your local computer. For example, when I selected the master branch as my current branch, here's what several directories looked like:

![Master branch directory](images/master-branch-directory.png)

You can see that the pylesson directory has a lot of files in it and the lod directory doesn't.  If I change to the "gh-pages" branch:

![Change to gh-pages branch](images/change-to-gh-pages.png)

then I'm checking out a different set of files.  Here's what the directories look like now:

![gh-pages branch](images/gh-pages-branch.png)

Some files have disappeared, like the ones in the pylesson directory, and other files have appeared in the lod directory.  The content of the files themselves may also change.  So it's important before you start working on files that you are clear what branch you currently have checked out.  

## Deciding how to work

Although Github is designed for collaboration, it can be a useful tool even if you are working on something by yourself.  It provides a way to track your editing progress by versioning and makes it possible to revert to an earlier version if you really mess something up.  It's also a way to access your work on different computers.  Things get more complicated when you are working with others.

There are several ways you can work in your own repository or when collaborating in a shared repository.  There are additional options if you are working on an open source project where contributors don't have write access to the repository, but we'll talk about them in the next session.

If you are working by yourself creating a new document, or if you are making trivial changes, you may opt to edit the master branch directly.  However, if you are on a team and making substantial changes, or if you are working by yourself and are concerned that the changes you are making may not work out, it's better to create a separate branch and work on that.  Similarly, if changes are extensive and it will take a while to finish them, you will probably want to leave the master branch in a stable state until you've finished the changes.  You can then merge them into the master branch all at once to create a new version of it.  

In any case, before you can edit an existing document, you will need to decide on a branching strategy.   The number of branches also can influence the probability of creating merge conflicts when edits are made to a version that isn't the most recent one. When there are few branches with many people working on them, merge conflicts are more likely.  If there are more branches with fewer people working on each one, merge conflicts of this sort are less likely to arise.

![GitHub work cycle](images/work-cycle.png)

## Work cycle

When you are editing files using GitHub desktop, it is important to have a disciplined work cycle to make sure that your work gets saved to the hub without merge conflicts. After you've decided what branch you need to work on, it's very important to make sure at the start that you are working on the most recent version of it by pulling any changes from Github. Click on the Fetch origin button at the upper right of the window.  If there are changes that need to be downloaded, you'll see a small number by a downward pointing arrow.  Click the button (now labeled "Pull origin") again to download those changes.

![Download changes](images/download-changes.png)

If you forget to update your local copy of the branch, you risk creating a conflict, since you may be working on a copy that isn't the most recent one.

Let's open a text editor (Use Notepad today, but I recommend installing ATOM, [https://atom.io/](https://atom.io/), for your personal use).  Navigate to the location where you checked out the repo.  Make some changes to the _**TakeAways.md**_ file, then save it.  If you click on the Changes tab at the upper left of the window, you should see the files that changed since the last update and clicking on a filename will show the kind of changes at the right of the screen.  

![File changes](images/file-changes.png)

Commit your changes.  You'll then see the new commit in the history and as a change that's ready to push up to GitHub.

![Make commit](images/make-commit.png)

 Click on the **Push origin** button to push your changes from the desktop client to GitHub.com.

## Resolving a conflict that occurs when pushing

Sometimes when you attempt to push a commit, you have an unpleasant surprise: a warning saying that the repository has been updated since your last pull.

There are two common ways that this can happen. Sometimes I've been working on a document on one computer, then start working on it on a different computer having forgotten to pull the most recent commits from GitHub. Another possibility is that you've been working on a document for a long time, and during that time, a collaborator made changes to the same document and pushed them to GitHub before you made your changes.  

In the following example, my alter ego and collaborator, Tomy the Cat, has edited the Python script we were working on while I was editing it.  

![Conflicted change 1](images/first-conflicted-change.png)

However, I was working offline in a text editor and changed the added number to 1 instead of 5.  

![Conflicted change 2](images/second-conflicted-change.png)

Here's what happened when I tried to push my changes:

![Repo is outdated](images/repo-outdated.png)

The problem is pretty easy to fix if I've been using Atom as my text editor.  Here are the steps to fix the problem:

Go to the Repository menu and select Pull.

![Pull the repo](images/pull-repo.png)

I will then get a popup message like this:

![Conflict warning](images/conflict-detected.png)

If I click on the "Open in Atom" button, I'll get this screen in the Atom editor:

![Choose conflict](images/choose-conflict.png)

The editor presents me with a choice between my change and Tomy's change.  Of course I'm right, so I pick my change.  Now the popup has changed:

![Choose conflict](images/conflict-fixed.png)

and I can now commit the resolved file.

## A better way to manage changes

When Tomy wanted to change the code, instead of committing his change directly to the master branch, he could have created a new branch.

![Create branch for change](images/create-branch-change.png)

After the "patch" branch is created, a new page opens to create a pull request:

![Create pull request](images/create-pull-request.png)

Notice that the pull request includes an "@mention" with the my username.  That generates an email to the collaborator:

![Email generated by request](images/pull-request-email.png)

Clicking on the link to view the diff shows how the two branches differ:

![Online diff](images/online-diff.png)

The collaborator can follow the link in the email to the pull request dialog and approve the change if they want.

![Pull request dialog](images/branch-pull-request.png)

After clicking Merge pull request, there's a confirmation and opportunity to comment.

![Confirm merge](images/confirm-merge.png)

A happy ending! The change was made without conflicts!

![Confirm merge](images/successful-merge.png)

Let's imagine a less happy ending. Perhaps I didn't see Tomy's email about the pull request and had gone ahead and made my change directly to the master branch before merging his patch branch.  That's generated a conflict that now shows up in the pull request dialog.

![Confirm merge](images/pull-request-merge-conflict.png)

Clicking on the Resolve conflicts button brings up the online editor showing where the conflicts lie:

![Confirm merge](images/online-conflict-resolution.png)

After editing the document so that the conflict is gone, click the Mark as resolved button, then click Commit merge.

![Confirm merge](images/online-conflict-resolved.png)

This merges the modified, unconflicted branch into the patch branch.  You'll then go back to the pull request screen and have an opportunity to merge the patch branch into the master branch. The pull request can then be merged and the patch branch deleted.

The creation of pull requests and resolving conflicts between branches can also be done offline, but the nice, linear record of the pull request history is best seen online.


### For more tutorials and resources about using GitHub visit:
**GitHub Guides** [https://guides.github.com/](https://guides.github.com/)
**GitHub Training & Guides** [https://www.youtube.com/user/GitHubGuides/featured](https://www.youtube.com/user/GitHubGuides/featured)
**GitHub Help** [https://help.github.com/](https://help.github.com/)
