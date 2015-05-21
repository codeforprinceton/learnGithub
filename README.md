# learnGithub
Repo for learning Github - used at our hacknights

## How to use Git and Github

You and Person A want to work on a project together. The project
you want to work on is already on Github. You are new to this
collaboration thing.

    - Installation: http://git-scm.com/book/en/v2/Getting-Started-Installing-Git

## Making changes via Github:
  0. Make a Github account.

  1. Visit the Github project on a browser.

  2. Open the file.

  3. Make a change. Because you are not a collaborator, it will "fork" a copy
     of the repo. This means that you are making a copy of the project on
     Github and it's going to be associated to your account.

  4. Submit a pull request. By doing so, you are asking the maintainers
     of the project to review your changes, and that you are requesting for
     them to merge it back into the repository that they are maintaining.

  5. A collaborator on Github will then review the changes.
    5a. If the collaborator likes it, then that person can *accept* the
        pull request, and vice versa.

## Making changes via Github for Mac (or Windows):
  0. Login with your Github account.

  1. Visit the project via a browser and click the "Clone in Desktop"
     button at the right.

  2. Make changes using a text editor (like Vim, Emacs, Atom, Sublime, etc.)

  3. Once you are done with the changes, go back to Github for Mac, and
     make sure you are under the "Changes" tab.

  4. Commit your changes.

  5. Press the "Pull Request" icon (at the left of "Sync")

## Making changes in the Terminal (Mac/Linux):
  1. Install `hub`. See: https://hub.github.com/

    a. You want `hub` to be used when you use `git` in the command line.
        You can do that by editing your `.bashrc` or `.bash_profile` in
        the directory and adding the line `alias git=hub` using a text
        editor.
    b. Save your changes.

    c. Go back to the terminal and let it know about the change you've
       made: `source ~/.bash_profile` or `source ~/.bash_rc` if you've
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

  7. Stage your changes. `git add .` (The "dot" refers to the current directory).

  8. Commit: `git commit -m "my commit message"`

  9. Fork the repository, which will make a copy of the project and save it
     under your account on Github: `git fork`

  10. Push to your new remote: `git push <YOUR_GITHUB_NAME>`

  11. Make a pull request. `git pull-request`
