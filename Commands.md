# Git

**DELETING FILES**

     Command : git rm fileName               (delete both local and GitHub)
               git commit -m "Deleted"
               git push 

               git rm --cached fileName      (delete only from GitHub)


**TAGGING**

     Command : git tag -a v1.0 -m "message"       (create a tag)
               git tag                            (show tag)
               git tag show v1.0                  (show tag details)
               git push origin v1.0               (push tag to GitHub)

               git tag -d v1.0                      (delete tag locally)
               git push origin --delete tag v1.0    (delete remote tag)