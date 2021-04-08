# Contribution in the QuasarApp group.

## Issues
1. Any developer has the right to choose any unassigned issue. If the developer has assigned tasks, then he must solve them first.
2. If developer find any problems when works time on another issue he must be create a new issue in a works project.
3. All issues must be solve in a separate branch. 
4. The branch must be named using next template:
    > **task_XXX** - where **task_** are mandatory part of the branch name, and **XXX** are number of a solving issue.
  

## Pull Requests

When developer are begin work on selected issue then he must be create a pull request with name of the solving issue. 

1. The name of the pull request must be marked as a [WIP] (Work In Progress) if the developer still works on a selected issue.
2. When developer finished work on issue he must be remove WIP marker.
3. The discription of the pull request must be contains the **fix #XXX** label. 
4. If The pull request contains difficult solution or changes then a description of the pull request must be contains detailed description of the all changes in a code.
5. If the project have a releases branch then all pull requests must be checkout from the release branch marked in the issue milistones.
    > For example CQtDeployer have issue in the **1.6 milistone** then developer must be checkout from the **v1.6** branch and create pull reqest from own **task_XXX** branch to the **v1.6** branch. 


## Commits 
Descriptions of commits
1. All commits must be contains the **ref #XXX** label for automaticly including commits to solving issue. 
2. The **fix #XXX** label is forbidden because all commits should be pass all CI tests and review of another developers.
3. If commit do not have a any issues then commit should be contains detailed description about changes.


# And good luck it will be useful to you 😉 
