# Git

**DELETING FILES**

     Command : git rm fileName                (delete both local and GitHub)
               git commit -m "Deleted"
               git push 

               git rm --cached fileName       (delete only from GitHub)


**CLONING**

     Command : git clone repository-URL       (clone code from repository to local)


**TAGGING**

      Command : git tag -a v1.0 -m "message"         (create a tag)
                git tag                              (show tag)
                git tag show v1.0                    (show tag details)
                git push origin v1.0                 (push tag to GitHub)

                git tag -d v1.0                      (delete tag locally)
                git push origin --delete tag v1.0    (delete remote tag)


**BRANCHING (A separate line of development inside project , doesn't affect main code)** 

      Command : git switch -c branchName                    (create new branch)

                git switch main                             (switch to main branch, cant delete branch without switching to main)
                git switch -                                (switch to previous branch)


                git branch -d branchName                    (delete branch locally)
                git push origin --delete branchName         (delete from GitHub)


**OTHERS**

      Commands : git log                                 (check past commits) 

                 git diff                                (shows the changes made)
                 git diff commit1 commit2
                 git diff main feature-branch