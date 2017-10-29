# Git Workflow
This is a tutorial about the Git Workflow on GitHub, which is also called Githubflow.

The Githubflow has only one `master` branch. You should develop on your own `feature branch` and merge it to the `master` after work.  

This is the flow that Github provides.
![](images/Githubflow.png)
***
## 1.  Githubflow

The core idea behind the **Githubflow** is that all feature development should take place in a dedicated branch instead of the `master branch`. This encapsulation makes it easy for multiple developers to work on a particular feature without disturbing the main codebase. It also means the master branch will never contain broken code, which is a huge advantage for continuous integration environments.
![](images/git-workflow-feature-branch-1.png)

Encapsulating feature development also makes it possible to leverage `pull requests`, which are a way to initiate discussions around a branch. They give other developers the opportunity to sign off on a feature before it gets integrated into the official project. Or, if you get stuck in the middle of a feature, you can open a `pull request` asking for suggestions from your colleagues. The point is, `pull requests` make it incredibly easy for your team to comment on each other’s work.


## 2. How it works                                                                                                                                   


The Feature Branch Workflow assumes a central repository, and master represents the official project history. Instead of committing directly on their local `master` branch, developers create a new branch every time they start work on a new feature. Feature branches should have descriptive names, like animated-menu-items or issue-#1061. The idea is to give a clear, highly-focused purpose to each branch. `Git` makes no technical distinction between the `master` branch and feature branches, so developers can edit, stage, and commit changes to a feature branch.
 

In addition, feature branches can (and should) be pushed to the central repository. This makes it possible to share a feature with other developers without touching any official code. Since `master` is the only “special” branch, storing several feature branches on the central repository doesn’t pose any problems. Of course, this is also a convenient way to back up everybody’s local commits. The following is a walk-through of the life-cycle of a feature branch.

