# Week 4






## Workflow for creating a new local repo and syncing it to a new Github repo

-   create local repo folder
-   `git init` — initialises the repo
-   create repo on GitHub
-   `git commit -m "first commit"` 
- `git branch -M main` — renames current branch (always master by default) to *main*
-   `git remote add origin <link to github repo e.g. <https://github.com/farahc123/tech501-week2.git>>` — specifies the remote repo (e.g. a github repo, which is the *origin*) so you can create, view, and delete connections to it
-   ` git push -u origin <branch name e.g. main>` — does the first sync of the files and commit history to the previously added remote repo
