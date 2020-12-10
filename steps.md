
GitHub is a development platform that helps to collaborate, share, manage, and build projects in a better way. It is used to store the source code for a project and track the complete history of all changes to that code. It allows developers to collaborate on a project more effectively by providing tools for managing possibly conflicting changes from multiple developers. 

Important terms you must be aware of:
•Fork 
•Clone
•Pull request
•Branch
•Merge

 

 


GitHub Scenarios



Pull a specific file



1.Fork the repository.
2.Clone the repository:

 










git clone https://github.com/YOUR-USERNAME/RS8-mde-enabler/mde-docs.git  (Path from your forked branch) 
 


 

   3. Go inside your workspace in local machine:

        For example, D:/GitHub/mde-docs (Your workspace in local machine)

   4. Verify your origin:

 









git remote –v
 


 
   5. Add upstream:
(This step must be done only once. If there are multiple upstream set, then it is recommend to remove them first (Samsung repo). )









  

git remote add upstream https://github.sec.samsung.net/RS8-mde-enabler/mde-docs.git
 


   6. Verify your origin and upstream:

 









git remote –v
 


    7. Sync the upstream repository files to your local machine:









git fetch upstream
 


   8. Go into your master branch:









git checkout master
 


   9. Pull the specific file from a PR:









git fetch upstream pull/ID/head:<BRANCH NAME>   (give a new branchname)
 


   10. Go into the new branch:









git checkout <branch name>
 


 

You can find the specific file in your respective folder.

 


Create a PR




When you want to merge an edited file to the master repository, raise a pull request. To create a PR:




1.Clone the repository:










git clone https://github.com/YOUR-USERNAME/RS8-mde-enabler/mde-docs.git  (Path from your forked branch) 
 



2.Go inside your workspace in local machine:

For example, D:/GitHub/mde-docs


3.Verify your origin/upstream:

 









git remote –v
 



4.If upstream not available, then add upstream:

 









  

git remote add upstream https://github.sec.samsung.net/RS8-mde-enabler/mde-docs.git
 



5.Sync the upstream repository files to your local machine:

 









git fetch upstream
 



6.Check whether your master branch and the main master branch is even.


7.If the main master branch is even, got to your master branch:

 









git checkout master
 



8.Copy and paste your edited file into your workspace in your local machine and check the status:

 









git status
 



9.The added file names will be displayed in red color.


10.Add the files:

 









git add .
 



11.Verify the status:

 









git status
 


 

If the files are added then the file names will be displayed in green color.


12.Verify whether your name and changes are proper or not (Optional):

 









gitk
 



13.   Commit your changes to be pushed:

  









git commit -m "Add a meaningful message"
 


 

 

   14. Push your file:


 









git push origin 

  

or

  

git push origin master
 


 

 




   15. Go to GitHub site and create a new pull request.

   16. Compare across fork:

          Base: HQ and Master: your repo

   17. You can see your added files and the changes.

   18. Give comments and create new pull request.

   19. Verify whether a new pull request is raised or not. If raised whether all changes are updated.

   20. If you have missed any changes, click the pencil icon in the top right end. Edit your file in UI itself and commit the changes. (Recommended for small changes).

   21. You can edit your file and follow the same steps to push it from your local machine using Git bash.





Files not found even after cloning and syncing




 

If you do not have, your required file even after cloning and synchronizing your files with upstream. This issue is because your fork is an older version of the main repository. 

 



 

Perform these steps only if you do not have any open PRs. There is a chance of automatic closure of the PRs.

Here you can either delete the forked repository or start afresh or can use the following commands:

 









git remote -v
 










git reset--hard upstream/master 
 



 


Use the third step, only if you have to push the changes to your master. 









git push --force origin master 

  
 


Now check your repository you will get the file. This is the recommended way.

 

 


 


 

Deleting the forked repository is not a good practice as the history of your work on Git repository will be erased forever. 




 


How to raise multiple PRs 



 
If you have to raise multiple PRs simultaneously without affecting each other, create PRs from different branches.

If you have cloned the repository, then please follow the steps from 1 to 7 in Create a PR.

From master branch, create a new branch










git checkout –b <new branch> 
 


 

From the new branch raise a PR.

If you want to raise another PR, go to master branch:









git checkout master
 


 Now create a new branch and raise a new PR. You can create any number of PRs without affecting each other.


Rebase PR




Merge Conflicts

From Catherine,

The steps to resolve the Merge Conflict (In this follow we are considering you are to fix master branch) :


 - Checkout to the base branch that you are trying to fix (master in this case)
 - Get the latest version ("git pull", or "fetch upstream, merge upstream/master master", and so on)
 - Checkout to the branch you are working
 - git rebase master (syncing the latest master branch to your working branch. If you have conflict it shows the error log and stops.)
 - The consol log will let you know which file, and where to fix to resolve the conflict with >>>>/ <<<< mark
 The >>>> and <<<<< show the diff of your work and the master branch file.
 - Check the conflict and fix it.
 - git add MODIFIED_FILE
 - git rebase --continue 
 - git add MODIFIED_FILE (repeat this step until every files are fixed)
- git push origin YOUR_WORKING_BRANCH -f  

 

From Kang,

Please do git rebase, update new changes, and push a commit.

How to rebase:

$ git fetch upstream
$ git checkout master
$ git merge upstream/master master
$ git checkout opentk-docs
$ git rebase master

change according to review comments

commit and push to github:
$ git commit -a ( or git commit -a --amend)
$ git push origin opentk-docs

 

For more information, see #485


git commit --amend




If you want to update the PR (fix the contents, adding images, etc), you can use git commit --amend

In the work space
1.Fix the contents (update contents, fix markdown tags, and so on).
2.Use git add to add the updated files.
3.git commit -a --amend
With this, you can update the commit you made.
4.git push origin your_working_branch -f
This will forcibly update your commit in your repository, also this related PR.

With this commands, you don't need to close your PR and create new PR every time to apply a fix.
You can update these PRs.
 
  


Revamp




Target is to revamp a doc content and raise a PR over an existing doc folder.

The following steps are related to Tizen revamp; hence, all the files will be using in Tizen file names.

Note that we were just revamping Tizen Studio. All other docs were kept intact.

Following commands helps you to create a replica of the existing file structure and it creates a mirror folder of the same file:










$ cd tizen-docs     $ git checkout -b tizen-studio-update

$ cd docs/application

$ cp -arf tizen-studio tizen-studio-0

$ git add tizen-studio-0

$ git commit -a

$ git push origin tizen-studio-update 
 


   

And then click "New Pull Request" in UI.

 

In the following example, the end result is to create a mirror folder of docs/application/tizen-studio by raising a PR and then add all the newly added and modified files to the mirror path.

To do this, follow these steps:

In Tizen repo:
1.Copy docs/application/tizen-studio.
2.Add docs/application/tizen-studio-0.
3.Create a pull request for the same in the repo.
4.Edit files in tizen-studio-0 directory.
5.Rebase the PR with all the changes.
6.Create docs/application/toc_tizenstudio.md for updating TOC.
7.Update links to tizen-studio in other guides, for example, ../../tizen-studio-0/setup.md. Use the following grep command to list out the links in all the folders.

Text to search:  Grep –r –n “termtoserach” &> list.txt 
File name to search: Grep –r –n “filename.html” &> list.txt         
Grep –r –n “filename.md” &> list.txt 


8.Mark all the title and sub title changes made in the pages in an excel sheet, with old title and new title.


9.Apply all the changed titles in the related docs to prevent broken links.
10.Update docs/application/toc_applicaton.md as toc_tizenstudio.md.
11.Merge all changes under tizen-stuido-0 to master branch.

 

In Tizen Developer Site:
1.Create a new document of which title is "Tizen Studio" on Tizen Developer Site.
Drupal will create a new URL not to conflict the URL: it will be https://developer.tizen.org/development/tizen-studio-0/.
2.Update links to tizen-studio in other guides. Links will look like https://developer.tizen.org/development/tizen-studio-0/install.
3.Complete checking broken links and other errors on TD.
4.Disable old Tizen Studio menu not to show public (https://developer.tizen.org/development/tizen-studio/).
5.Disable old Tizen Studio menu not to show public (https://developer.tizen.org/development/tizen-studio/).
6.Publish all new documents under https://developer.tizen.org/development/tizen-studio-0/.
7.Delete old Tizen Studio files not to search by Google. (https://developer.tizen.org/development/tizen-studio/) 


Points to be taken care of:
•Adherence to style guide
•Follow grammar guidelines
•No spelling mistakes
•No image breaks
•No broken links

  


Your fork is uneven with the main master



 
If your fork is not even with the main master branch, use the following commands:



 


You can perform these steps even if a PR is opened.









git fetch upstream
 










git merge upstream/master master
 










git push origin master
 










git checkout –b <new branch>
 
