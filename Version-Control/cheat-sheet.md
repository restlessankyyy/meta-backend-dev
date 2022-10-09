## Git Cheat Sheet

Git is the open source distributed version control system that facilitates GitHub activities on your laptop or desktop. This cheat sheet summarizes commonly used Git command line instructions for quick reference.
services@github.com
services.github.com

*GitHub for Windows*
<https://windows.github.com>
*GitHub for Mac*
<https://mac.github.com>
*Git for All Platforms*
<http://git-scm.com>
Git distributions for Linux and POSIX systems are available on
the official Git SCM web site.

#### Install

*Configure tooling*

Configure user information for all local repositories

Enables helpful colorization of command line output

```$ git config --global color.ui auto```

Sets the email you want attached to your commit transactions

```$ git config --global user.email "[email address]"```

Sets the name you want attached to your commit transactions
```$ git config --global user.name "[name]"```

Clone (download) a repository that already exists on GitHub, including all of the files, branches, and commits

```$ git clone [url]```

*Create repositories*

When starting out with a new repository, you only need to do it
once; either locally, then push to GitHub, or by cloning an
existing repository.

Turn an existing directory into a git repository

``` $ git init ```

Updates your current local working branch with all new
commits from the corresponding remote branch on GitHub.
 git pull is a combination of git fetch and git merge

``` $ git pull ```

*Synchronize changes*

Synchronize your local repository with the remote repository
on GitHub.com

Uploads all local branch commits to GitHub

``` $ git push ```

Combines remote tracking branch into current local branch

``` $ git merge ```

Downloads all history from the remote tracking branches

``` $ git fetch ```

Deletes the specified branch

``` $ git branch -d [branch-name] ```

Combines the specified branch’s history into the
current branch. This is usually done in pull requests,
but is an important Git operation.

``` $ git merge [branch] ```

Switches to the specified branch and updates the working directory

``` $ git checkout [branch-name] ```

*Branches*

Branches are an important part of working with Git. Any
commits you make will be made on the branch you're currently
“checked out” to. Use git status to see which branch that is.

Creates a new branch

``` $ git branch [branch-name] ```

*The .gitignore file*

Sometimes it may be a good idea to exclude files from being
tracked with Git. This is typically done in a special file named
 .gitignore . You can find helpful templates for .gitignore
files at github.com/github/gitignore.

Want to learn more about using GitHub and Git?
Email the Training Team or visit our web site for learning
event schedules and private class availability.

#### Training

*git*: an open source, distributed version-control system

*GitHub*: a platform for hosting and collaborating on Git repositories

*commit*: a Git object, a snapshot of your entire repository compressed into a SHA

*branch*: a lightweight movable pointer to a commit

*clone*: a local version of a repository, including all commits and branches

*remote*: a common repository on GitHub that all team member use to exchange their changes

*fork*: a copy of a repository on GitHub owned by a different user

*pull request*: a place to compare and discuss the differences introduced on a branch with reviews, comments, integrated tests, and more

*HEAD*: representing your current working directory, the HEAD pointer can be moved to different branches, tags, or commits

*Make changes*

Browse and inspect the evolution of project files

Lists version history for the current branch

``` $ git log ```

Lists version history for a file, including renames

 ``` git log --follow [file] ```

 Shows content differences between two branches

 ``` $ git diff [first-branch]...[second-branch] ```

Outputs metadata and content changes of the specified commit

 ``` $ git show [commit] ```

Snapshots the file in preparation for versioning

``` git add [file] ```

Records file snapshots permanently in version history

``` $ git commit -m "[descriptive message]" ```

*Redo commits*

Erase mistakes and craft replacement history

Undoes all commits after [commit], preserving changes locally

``` $ git reset [commit] ```

Discards all history and changes back to the specified commit

``` $ git reset --hard [commit] ```

---- ---- ---- ----
