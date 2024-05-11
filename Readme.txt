1. `git init` -> Powers your folder to be managed by git, and initialises a new empty repository.
It also creates a .git folder that has all the relevant logic to manage versions of your project.

2. `Working Area` -> There can be a bunch of files that are not currently handled by git.
It means tgat changes done or to be done in those files are not managed by git yet.
A file which is in working area is considered to be not in the staging area. 
When we do `git status` and we see abunch of `untracked files` then these are actually 
called to be in the working area.

3. `Staging Area` -> What all files are going to be part of the next version that we will 
create. This staging area is the place where git knows what changes will be done from the 
last version to the next version.

4. `Repository Area` -> This area actually contains the details of all your previous 
registered versions. And the files in this area, git already manages them and knows their
version history.

5. `git add <filename>` -> moves file from working area to staging area.

6. `git rm --catched <filename>` -> moves file back from staging area to working area.

7. `commit` -> Commit is a particular version of the project. It captures a snapshot
of the project's staged changes and creates a version out of it.

8. `git commit` -> registers staging changes to a commit.
    a new terminal will be opened press 'i' and now we are able to commit here,
    for ex: "This is my first commit."
    now press "Esc" + ":wq" + "enter".
    Out first commit is done.

9. `git log` -> list downs all the commits of the repository. If you want to exit out
of git log prompt press 'q'. 

10. `git restore <filename>` -> It removes all file changes from the staging area to be 
committed. This can be useful, if we did some dirty piece of code and now nomore want it.
Instead of deleting every change line by line, we can restore it or you can say restore 
last clean version of the file.

11. `git restore --staged <filename>` -> It removes file from changes from staging area to
the working area. This only works if changes are in your staging area.

12. Diff between git rm and git restore
ans. If we want to move the whole file back to the untracked state, then we do git rm,
otherwise if we just want the changes to moved in working area or staging area we use 
git restore.

13. `git diff commitID1 commitID2` -> gives the difference of all file changes between 
two commits.

14. `git commit -m "<our commit msg>" -> If we want to avoid opening a text editor like 
vim/nano to add commit msg we can use this following command.

15. `git remote` -> list down all the remote connection names.

16. Remote connection -> It helps you to link two git repos. for uploading and downloading 
changes from each other.

17. `git remote add <name of remote>` <<link of the remote> -> this command helps us to 
add a new link toh the remote repo. and give a name to it.

18. `git remote rm <name of remote>` -> this command deletes a remote connection.

19. `git remote rename <oldname> <newname>` -> this command renames the remote connection

Note: The name of the remote connection is always used to establish communication between 
the repos.