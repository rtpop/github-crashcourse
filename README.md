# Git and GitHub crash course
This is a repository for the practical component of a git & GitHub course. This includes a short presentation of gi and the main features of git, as well as a more detailed guide of the basics of git and GitHub. 

Slides:
https://docs.google.com/presentation/d/1pOj41FHSDqTLEfji0Nqh9-PoDVcq861yObhCFfQM0TU/edit?usp=sharing

# Contents

- [Git and GitHub crash course](#git-and-github-crash-course)
- [Contents](#contents)
  - [Git and GitHub basics](#git-and-github-basics)
    - [Adding files](#adding-files)
    - [Committing](#committing)
    - [Pushing and pulling](#pushing-and-pulling)
    - [Branches](#branches)
    - [Cloning a repository](#cloning-a-repository)
    - [Forking a repository](#forking-a-repository)

## Git and GitHub basics
Git is a widely used version control system designed to track changes made to files within a repository. It was primarily designed for programming, but it can be used to version control any document. Services such as GitHub are a great way of collaborating on projects or even backing up your code or other important documents while tracking any changes made for future reference. GitHub has a [comprehensive tutorial](https://docs.github.com/en/get-started/start-your-journey) on how to use git with GitHub, along with some practical exercises. Here, I will only briefly describe the main concepts. I will primarily go over how to use the web based GitHub service as well as use git locally via command line. However, if you are not comfortable with using command line, there is also a [GitHub desktop application](https://desktop.github.com/download/). Although that is outside the scope of this tutorial, many of the features of the desktop app are similar to the web based version.

### Adding files
In order for git to track a file, it must first be added to the repository. When creating a file directly on GitHub, it will automatically be added to the repository. However, if you create a file locally, you must first add it by opening a terminal and using the ```git add``` command.

```function test()
git add your_file_name
```

You can add multiple files at once, or even the entire repository.

```function test()
git add your_file_name your_other_file_name
```

```function test()
git add .
```

You must [commit](#committing) added files as you would any other change.

### Committing
Commits are the backbone of git and are how we can track changes made to any file. Every time you make a new commit, you have to include a commit message. Each commit is assigned a unique ID, so it can be found at any point and the changes committed in that commit can be seen. If you edit a file on GitHub directly, it will automatically commit when saving changes and prompt you for a commit message. You can also commit manually by pressing the green ```Commit changes``` button.

<img src = images/commit.png>

<br>

To commit via command line on your local machine, open a terminal, navigate to your repository and use the following command.

```function test()
    git commit your_file_name -m "Your commit message"
```

It is also possible to commit multiple files at once.

```function test()
    git commit your_file_name your_other_file_name -m "Your commit message"
```

Or commit all changed files in the repository, although this is typically not recommended. It is best practice to keep commits small and frequent so you can easily track each change and the purpose of that change. This is especially important for colaborative code where someone else might need to understand what changes you made and why (but it is also incredibly useful for your future self!). 

```function test()
    git commit . -m "Your commit message"
```

### Pushing and pulling
Pushing and pulling is how we can sync the local and remote repositories. We can push any changes we make locally to the remote repository only if they have been committed first. When pushing an pulling, git will check for conflicts between the loal and remote versions to avoid overwriting information. If it cannot automatically resolve the differences between the two versions without any loss of information, it will require you to manually resolve it by choosing which version to keep. This is especially important when working in collaboration and this is why using [branches](#branches) is important. 

To push and pull, use the following commands. Make sure you are in the directory where your repository is stored.

```function test()
git pull
```
```function test()
git push
```

Alternatively, you can use the full path to your repository to push/pull from a different location.

```function test()
git pull /path/to/your/repository
```
```function test()
git push /path/to/your/repository
```

It is also possible to only push some files.

```function test()
git push your_file_name
```

### Branches
Branches are 

### Cloning a repository
Cloning a repository means creating a copy of a remote repository on your local machine and linking it to the remote repository, so that any changes made can be communicated between the local and remote repositories via pushing and pulling. You can clone any public repository or private repository you have access to, but you will only be able to

First, make sure you have git installed on your computer. You can download git for your operating system from the [git website](https://git-scm.com/downloads).

Next, get the link to the repository by clicking the ```Code``` button and copying the link. You can choose between ```HTTPS```, ```SSH``` or ```GitHub CLI```. For most cases, ```HTTPS``` is a good option.

<img width="511" height="402" alt="image" src="https://github.com/user-attachments/assets/d1909c78-7871-4df7-b564-ab5d16a6a487" />

<br>


On your local machine, open a terminal and run the command below. make sure you navigate to a directory where you want the repository to be cloned.

```function test()
  git clone https://github.com/rtpop/github-crashcourse.git
```

To open a terminal on Windows press the Windows key on your keyboard or click on the Widows button in your taskbar. Type ```powershell``` in the search bar. 


### Forking a repository
Repository forking is a GitHub feature that allows users to create copies of public repositories in their own accounts. This means that they can make changes to the contents of the repository without needing permission to the original repository. These changes can later be merged with the original repositories via pull requests, which we will discuss next. 

To fork a repository, simply click on the fork button in the upper right corner.

<img src = images/fork.png>

<br>

This will take you to a forking page where you can customise the name of your repository and some other settings.

<img src = images/fork-2.png>

<br>

Author:
Romana Pop
