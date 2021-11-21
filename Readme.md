# Git

`Most of these ideas and examples are from @codediodeio. One of my favorite YouTuber Fireship` [Link](https://www.youtube.com/watch?v=HkdAHXoRtos&t=285s)

## Version Control System

- a system for managing your files
- from state of chaos to stability
- create multiple branches and merge it to the main branch later

## Initialize git to start tracking your files

- `$ git init`
- this creates a hidden directory
- to completely remove the hidden file `$ rm -rf . or $ rm -rf .git`

## Pro Tip

- Install the `Gitlens` plugin in VScode
- **(Ctrl+Shift+P)** then type `git`, then selecet `Add Gitignore` to create a **(Plugin)** gitignore file to your project
- You can Stage and Unstage files by navigating to the `Source Control` and Click + right next to the file name
- It is always recommended to make small `Commits` to your branches to `AVOID Conflicts` when our code is getting larger and larger.

## Git Commands

- `$ git add <filename>` to `Stage` a certain file/files or `$ git add .` to add all `Unstaged` files
- `$ git branch` to check the current branch

## To create a branch for git

- `$ git checkout -b <name_of_branch>` to switch to a new branch **(NOTE)** there's no Double Qoutes to write the new branch

## To commit files on git

- If you want to save and not to `commit` your progress `$ git stash -u` this will stash your previous work and create a clean branch right after you type the code
- If you want to retrieve the saved stash `$ git stash pop`
- To commit files into git `$ git commit -m <your_message>` this will commit all the `staged` files into git

## To merge into the `main` branch

- To merge our current branch into the Main branch **(IMPORTANT!)** navigate first into the Main branch by searching it into the `Source Control panel` **(Ctrl+Shift+G G)** and then click the `More Actions` option **(... symbol)** and then select `Check Out to` and select `main`. Then we can now type into the terminal `$ git merge <branch_name>` to merge our `<branch_name>` to the main branch.
- We can also use the terminal code `$ git checkout -b main or $ git checkout main`**(If our main branch was commited)** to navigate to our main branch

## Git Merge flags

- If you have a lot of `unessesary or unrelevant commits` to a `<branch_name>` we can `squash` those commits down to have one single `merge commit message` to our main branch. So same as merging above, we navigate to the `main` branch and then `$ git merge <branch_name> --squash`.

## On Github

- To connect to our newly created `empty` remote Github repository `just follow Github's instruction` or `$ git remote add origin <repository_url>`
- To connect to a certain branch inside our `remote repository` or usually if it's empty we should just push our existing `local repository` type `$ git branch -M main`.
- To push our changes in our local repository to the remote repository `$ git push -u origin main`. 🚀🚀🚀
