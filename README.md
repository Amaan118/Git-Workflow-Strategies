
# Git Workflow Branches 

A brief description of how branching is perceived...  


### Git Flow: Main Branch

The purpose of the main branch in the Git flow workflow is to contain production-ready code that can be released.
In Git flow, the main branch is created at the start of a project and is maintained throughout the development process. The branch can be tagged at various commits in order to signify different versions or releases of the code, and other branches will be merged into the main branch after they have been sufficiently vetted and tested.


### Git Flow: Develop Branch

The develop branch is created at the start of a project and is maintained throughout the development process, and contains pre-production code with newly developed features that are in the process of being tested.
Newly-created features should be based off the develop branch, and then merged back in when ready for testing.


### Git Flow: Feature Branch

The feature branch is the most common type of branch in the Git flow workflow. It is used when adding new features to your code.
When working on a new feature, you will start a feature branch off the develop branch, and then merge your changes back into the develop branch when the feature is completed and properly reviewed.


### Git Flow: Release Branch

The release branch should be used when preparing new production releases. Typically, the work being performed on release branches concerns finishing touches and minor bugs specific to releasing new code, with code that should be addressed separately from the main develop branch.


### Git Flow: Hotfix Branch

In Git flow, the hotfix branch is used to quickly address necessary changes in your main branch.
The base of the hotfix branch should be your main branch and should be merged back into both the main and develop branches. Merging the changes from your hotfix branch back into the develop branch is critical to ensure the fix persists the next time the main branch is released.

**See below**

![Logo](https://1v5ymx3zt3y73fq5gy23rtnc-wpengine.netdna-ssl.com/wp-content/uploads/2021/03/git-flow.svg)


### some commands which deals with git branches  

1. ```git checkout <branch-name>```
> Checkout to the <branch-name> branch.  
  
2. ```git branch```
> List all branches.  

3. ```git branch -a```
> List all remote branches.
  
5. ```git branch <branch-name>```
> Create a new branch <branch-name> but remain in previos branch.  
  
6. ```git checkout -b <branch-name>```
> Create a new branch <branch-name> and checkout to the <branch-name>.

7. ```git branch -m <branch-name>```
> Rename the current branch to ＜branch-name＞.

8. ```git branch -d <branch-name>```
> Delete the specified branch. This is a “safe” operation in that Git prevents you from deleting the branch if it has unmerged changes.

9. ```git branch -D <branch>```
> Force delete the specified branch, even if it has unmerged changes. This is the command to use if you want to permanently throw away all of the commits associated with a particular line of development.

## For more info

 - [Git Flow Branch Strategy](https://www.gitkraken.com/learn/git/best-practices/git-branch-strategy#:~:text=The%20two%20primary%20branches%20in,feature%2C%20release%2C%20and%20hotfix.)

