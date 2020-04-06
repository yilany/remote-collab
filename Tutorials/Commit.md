# Git Commits

The most basic element in a Git history is called a _commit_. A commit consists of the changes made to a repository, along with a message describing the changes, information about who made the changes, and when the changes were made.

Creating a commit is a two-step process. First, you stage the changes that you want to commit, then you commit them.

💡 _By splitting up your work into bite-sized commits and crafting useful commit messages, you make it easier for yourself to navigate your own working process._

## Table of Contents

0. [Git Status](#git-status)
1. [Staging Commits](#staging-commits-git-add)
2. [Committing Commits](#committing-commits-git-commit)
3. [Next steps](#next-steps)

## Git Status (`git status`)

If you have made some changes to your project, it is always helpful to run the following command:

	git status
	
The `git status` command will give you a rundown of which files have been changed, and which changes have been staged to be committed.

## Staging Commits (`git add`)

While working on a project, you may make changes to one or more file. Before committing to making a commit, you can incrementally _stage_ the changes that you have made, or you can stage all of the changes at once.

The most common ways of staging commits are the following:

### `git add some_file_name`

To stage all of the changes made in a specific file, run the command `git add some_file_name`, with the name of the file replacing `some_file_name`.

### `git add .`

To stage the changes to all of the files in the current working directory, run the `git add .`.

### `git add -A`

To stage the changes to all of the files in the repository, run the `git add -A` command.

Once you have staged some changes, run `git status` again to see where you are at with the committing process.

💡 _The `git add` program has even more to offer. For more information, run the `git add --help`._

## Committing Commits (`git commit`)

Once you have staged changes to be made to a commit, now you have to _commit_ to committing the changes to your repository.

When making a commit, you _must_ submit a _commit message_. A commit message is a description of the changes you made to the repository. There are different style guidelines for crafting optimal commit messages, but [here is a good start](https://chris.beams.io/posts/git-commit/).

To make a commit, run the following command:

	git commit -m "Make a great commit message"
	
Here, you run the `git commit` program with the `-m` (i.e., with a message) option. Place your commit message in quotation marks.

💡 _As with all Git programs, run the `git commit --help` command to get a sense of all of your options._

## Next Steps

Now that you have staged and completed a _commit_ (🎉), you are ready to [push your changes to a remote repository](Push.md).
