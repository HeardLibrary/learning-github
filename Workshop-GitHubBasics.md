## Workshop I: GitHub Basics

## The Plan

1. Source Control, Git, and GitHub
2. Why Would I Want to Use GitHub?
3. The Basics of Markdown
4. Getting Started with GitHub
  * Creating an account
  * Creating a new repository from scratch
    * Branches, Commits, and Pull Requests

## Source Control, Git and GitHub

**Source Control**, the management of changes to documents, computer programs, large web sites, and other collections of information. Examples of source control tools:  Subversion, Perforce, Mercurial, Git...

**Git**, [http://git-scm.com/](http://git-scm.com/), is a version control system that tracks changes to files in a project over time. Git is a command line tool.

**GitHub**, [http://github.com](http://github.com), is a web-based Git repository hosting service with all of the revision control and source code management of Git plus some added features. GitHub provides a web-based graphical interface and desktop as well as mobile integration.  See GitHub repositories in action at [https://github.com/HeardLibrary](https://github.com/HeardLibrary)

## Why Would I Want to Use GitHub?

GitHub may describe itself as the place where software is built, but software developers and computer programmers are not the only people using GitHub.  Scholars in all disciplines are using GitHub to build digital projects, share data, and even using GitHub in the classroom. Below are some examples:

### Digital Projects

**Open Greek and Latin Project**, [https://github.com/OpenGreekAndLatin](https://github.com/OpenGreekAndLatin)
Produces machine-corrected XML versions of Greek and Latin works and translations.

**Syriaca.org: The Syriac Reference Portal**, [https://github.com/srophe](https://github.com/srophe)
A collaborative research project publishing online reference works concerning the culture, history, and literature of Syriac communities from antiquity to the present.

**LOGAR: Linked Online Gazetteer of the Andean Region**, [https://github.com/sawernke/gazetteer-demo](https://github.com/sawernke/gazetteer-demo)

**Corpus Baudelaire**, [https://github.com/HeardLibrary/corpus-baudelaire](https://github.com/HeardLibrary/corpus-baudelaire) TEI encoding of Baudelaire's *Le Fleur du Mal*.

### GitHub in the Classroom

**GitHub Education**, [https://education.github.com/](https://education.github.com/) Free and discounted plans for educational use. Faculty are using GitHub instead of a traditional course management system (Blackboard, Moodle, Sakai) or using GitHub as a submission platform for student assignments.

*Related Readings*

*The Emergence of GitHub as a Collaborative Platform for Education* [http://alexeyza.com/pdf/cscw15.pdf](http://alexeyza.com/pdf/cscw15.pdf)

*Push, Pull, Fork: GitHub for Academics* [http://www.digitalpedagogylab.com/hybridped/push-pull-fork-github-for-academics/](http://www.digitalpedagogylab.com/hybridped/push-pull-fork-github-for-academics/)

**COMP 116: Introduction to Computer Security**, [https://github.com/tuftsdev/DefenseAgainstTheDarkArts](https://github.com/tuftsdev/DefenseAgainstTheDarkArts)
Course website for COMP 116: Introduction to Computer Security

## The Basics of Markdown

Markdown, [http://daringfireball.net/projects/markdown/](http://daringfireball.net/projects/markdown/), is a lightweight and easy-to-use syntax for styling all forms of writing on the GitHub platform.

You can use Markdown for:
* Gists - a quick and easy way to share snippets of code with collaborators
* Comments in Issues and Pull Requests
* Editing the repository Wiki
* Files with a `.md` or `.markdown` extension such as the repository `Readme.md` file

GitHub.com uses its own version of the Markdown syntax that provides an additional set of useful features, many of which make it easier to work with content on GitHub.com. Visit the Mastering Markdown guide: [https://guides.github.com/features/mastering-markdown/](https://guides.github.com/features/mastering-markdown/)

## Getting Started with GitHub

GitHub is free to use for public projects.  A free account give you the ability to create an unlimited number of public repositories with an unlimited number of collaborators.  GitHub also offers a number of personal and organizational plans for those who need to collaborate on private repositories.

Creating your free account is the first step
![GitHub profile](https://i.imgur.com/3Oud0O2.png)

## Creating a New Repository

You have two options when creating a new repository.  You can click on the + next to your profile image in the top right corner of the screen or go to the repositories tab within your profile page and click the New button.

![Creating a new repository in GitHub](https://i.imgur.com/QbCm9bJ.png)

Just a few easy steps to initialize your repository:

1. Name it - Always keep it short and sweet.
  * Let's create a repository named **Hello-World**
  * Describe it (optional)
2. Select **Public** for your repository status
3. Check the box to initialize your repository with a README
4. Add a license
  * Your content will be publicly available.  A license will tell user how _**you**_ want your content to be used/ reused.
5. Click Create Repository!

![New Repository Form](https://i.imgur.com/mUYu2Hq.png)

### Let's Play with Your New Repository

* **Branching** is the way to work on different parts of a repository at one time. By default all new repositories are created with one branch named `master`. You can work within your master branch, but creating working branches allows you to develop a feature or idea and work out all the bugs before merging it into `master`(your production branch).
  * Go to your new repository `hello-world` and click the drop down at the top of the file list that says **branch: master**
  * Create a branch named `readme-edits`

![Create a Branch](https://i.imgur.com/6p6qt9D.png)

* On GitHub, saved changes are called **commits**.  Each commit has an associated **commit message** that describes the change being made and why.  These commits document the history of the repository.
  * We are currently in our working branch `readme-edits`, let's edit our README file by clicking on the pencil icon in the upper right corner of the README viewing pane. Make a change to the file and commit it!

![Edit README](https://i.imgur.com/F3472q4.png)

* **Pull Requests** are the key to collaboration on GitHub. Using a **pull request**, you are proposing changes and requesting that someone pull in your contributions. In GitHub, pull requests allow you to compare the content of two branches, and the changes, additions and subtractions are shown in green and red and called **diffs**.
  * Think of pull requests as a way to start a conversation where you can get feedback on the development process.  You can also use GitHub's @mention system to ask for feedback from specific people.
  * We're going to open a pull request for our own repository and merge it for practice. Click on the Pull Request tab and click on the green **Compare & pull request** button.

![Compare & Pull Request](https://i.imgur.com/yGFy2PR.png)

  * In your pull request, you are comparing the master branch with the changes you made in the readme-edits working branch. Create the pull request by clicking on the green **Create pull request** button.

  ![Create Pull Request](https://i.imgur.com/CLt0OUP.png)

* The last step is to put it all together and merge the changes in your `readme-edits` branch into the `master` branch.  Once your merge is complete you can delete your working branch.

![Merge Pull Request](https://i.imgur.com/JkQ9MMC.png)

Success!  You are now a GitHub user!

### For more tutorials and resources about using GitHub visit:  

**GitHub Guides** [https://guides.github.com/](https://guides.github.com/)  
**GitHub Training & Guides** [https://www.youtube.com/user/GitHubGuides/featured](https://www.youtube.com/user/GitHubGuides/featured)  
**GitHub Help** [https://help.github.com/](https://help.github.com/)
