# Git and GitHub crash course
This is a repository for the practical component of a git & GitHub course. This includes a short presentation of gi and the main features of git, as well as a more detailed guide of the basics of git and GitHub. 

Slides:
https://docs.google.com/presentation/d/1pOj41FHSDqTLEfji0Nqh9-PoDVcq861yObhCFfQM0TU/edit?usp=sharing

# Contents

- [Git and GitHub crash course](#git-and-github-crash-course)
- [Contents](#contents)
  - [Git and GitHub basics](#git-and-github-basics)
    - [Committing](#committing)
    - [Pushing and pulling](#pushing-and-pulling)
    - [Cloning a repository](#cloning-a-repository)
    - [Forking a repository](#forking-a-repository)

## Git and GitHub basics
Git is a widely used version control system designed to track changes made to files within a repository. Services such as GitHub are a great way of collaborating on projects or even backing up your code or other important documents while tracking any changes made for future reference. GitHub has a [comprehensive tutorial](https://docs.github.com/en/get-started/start-your-journey) on how to use git with GitHub, along with some practical exercises. Here, I will only briefly describe the main concepts. 

### Committing
Commits are the backbone of git and are how we can track changes made to any file. Every time you make a new commit, you have to include a commit message. Each commit is assigned a unique ID, so it can be found at any point and the changes committed in that commit can be seen. If you edit a file on GitHub directly, it will automatically commit when saving changes and prompt you for a commit message. You can also commit manually by pressing the green ```Commit changes``` button.

<img src = images/commit.png>

<br>

To commit via command line on your local machine, open a terminal, navigate to your repository and use the following command.

```function test()
    git commit your_file_name -m "Your commit message"
```

### Pushing and pulling
Pushing and pulling is how we can sync the local and remote repositories. 

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
