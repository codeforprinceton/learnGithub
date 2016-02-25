# learnGithub
--This comment makes this version far better than the original...
Repo for learning Github - used at our hacknights

## Scenario

You and a bunch of civic hackers want to work on a project together. The
project you want to work on is already on Github, such as this. You are new to
this social coding/collaboration thing and you want to make changes to a
project.

## Making changes via Github:

  1. Make a Github account.

  2. Visit the Github project on a browser.

  3. Open the file.

  4. Make a change. Because you are not a collaborator, it will "fork" a copy
     of the repo. This means that you are making a copy of the project on
     Github and it's going to be associated to your account.

  5. Submit a pull request. By doing so, you are asking the maintainers
     of the project to review your changes, and that you are requesting for
     them to merge it back into the repository that they are maintaining.

  6. A collaborator on Github will then review the changes. They will either
     accept the changes, or give advice as to improve the changes even more
     before accepting the changes.

## Making changes via Github for Mac (or Windows):

  1. Install Github for Mac (or Windows)

  2. Visit the project (such as `codeforprinceton/learnGithub`) via the browser
     and press `Fork`. This will make a copy of the repository and will store
     it under your account.

  3. Go to your fork of the project on Github. If you followed step 2, you will
     have it under `https://www.github.com/<YOUR_NAME>/learnGithub`.

  4. Click "Clone in Desktop" on the right.

  5. Make changes using a text editor (like Vim, Emacs, Atom, Sublime, etc.).

  6. Once you are done with the changes, go back to Github for Mac, and
     make sure you are under the "Changes" tab.

  7. Commit your changes by adding a summary and pressing `Commit`

  8. Press `Sync` to push your changes to your remote copy.

  9. Press the "Pull Request" icon (at the left of "Sync")

## Making changes in the Terminal (Mac/Linux):

  1. Install `hub`. See: https://hub.github.com/

    a. You want `hub` to be used when you use `git` in the command line.
        You can do that by editing your `.bashrc` or `.bash_profile` in
        the directory and adding the line `alias git=hub` using a text
        editor.

    b. Save your changes.

    c. Go back to the terminal and let it know about the change you've
       made: `source ~/.bash_profile` or `source ~/.bashrc` if you've
       made the changes there.

  2.  Change to the directory that you want to save the project to:

    a. `pwd` to list the current working directory.

    b. `ls` to list the files in the current working directory.

    c. `cd <some_directory>` to change the directory to `some_directory`

  3. Clone the repo: `git clone codeforprinceton/learnGithub`

  4. Check to see which branch you're in via `git branch`

  5. If you're in the right branch, you can fetch the most recent changes
     and merge it into your local copy of the branch through `git pull`

  6. Make your changes.

  7. `git status` to see all your changes.

  7. Stage your changes: `git add <name_of_file_you_changed>`
      - `git add .` is useful if you want to add multiple files.
        (The "dot" refers to the current directory).

  8. Commit: `git commit -m "my commit message"`

  9. Fork the repository, which will make a copy of the project and save it
     under your account on Github: `git fork`

  10. Push to your new remote: `git push <YOUR_GITHUB_NAME>`

  11. Make a pull request. `git pull-request "title of the pull request" -h
      <YOUR_GITHUB_NAME>:master -b codeforprinceton:master -f`
      - `-h` stands for `head`. The argument of it is where you want to take
        changes from.
      - `-b` stands for `base`. The argument of it is where you want changes to
        be applied.
      - `-f` stands for `force`. Useful for preventing errors. Without it you
        might get an error saying something like`Aborted: 1 commits are not yet
        pushed to origin/master`


## Useful links

- http://git-scm.com/book/en/v2/Getting-Started-Installing-Git
- https://www.udacity.com/course/how-to-use-git-and-github--ud775
