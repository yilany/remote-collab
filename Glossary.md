# Glossary of Terms

Here is a big list of terms you might come across in your adventures with Git and Github.

## Branch

A version of your [repository](#repository) which can diverge from another branch and also be merged into another branch. You are always working on some branch, whether it be the [`master`](#master-branch) or some other.

Create a new branch if you are working on any new feature. As soon as you are about to write any code or make any changes to a document, create a new branch! This provides a buffer between your fallible self and the current working version of your repository.

## Checkout

Switch to a different [branch](#branch) of a [repository](#repository).

For example:

	git checkout other-extant-branch
	
To create a new branch, you can run the following command:

	git checkout -b new-branch

## Clone

When working on a repository that is served online, one must first clone the entire repository to make a [local](#local) copy.

For example, to work on this repository, run the following command:

	git clone https://github.com/learninglab-dev/remote-collab
	
When cloning a repository, you bring down all of the files, as well as the entire history of each of those files.

## Commit

A change to a [repository](#repository). A commit is made on a [branch](#branch). Commits carry along with them information like when they were made, and who made them.

Making a commit requires the user to submit a [commit message](#commit-message) describing the changes made. Commit messages are often logged in a history, for easy browsing at a later date.

## Commit Message

When making a [commit](#commit), a message is required.

See these [guidelines](https://chris.beams.io/posts/git-commit/) so that you create the most helpful commit messages.

## Diff

The difference between any two [commits](#commit) in a [repository](#repository).  A diff consists of the smallest number of deletions and insertions needed to transform an earlier commit into a later commit.

Github displays a very nice color-coded representation of the requisite deletions and insertions when a [pull request](#pull-request) is created.

Creating a diff is based on solving the [longest common subsequence problem](https://en.wikipedia.org/wiki/Longest_common_subsequence_problem).

## Fetch

Bring down [commits](#commits) and [files](#files) from a remote repository without [merging](#merge) them.

## Fork

A [Github](#github) feature which allows you to [clone](#clone) a repository while updating the ownership of the new clone to you.

## Git

A distributed version control system. Created by Linus Torvalds for work on the Linux project.

Git employs the concepts of [branching](#branch) to track changes to a [repository](#repository) over time.

## Github

A web-based platform for sharing and collaborating on various types of documents.

It is built upon [Git](#git), and adds convenient features through its web-based user interface.

## Github Flavored Markdown

See [Markdown](#markdown).

## Init

To create a new [repository](#repository) in your current working directory, run the command:

	git init
	
This will create all of the necessary junk needed to track changes to your directory, including a single [branch](#branch) called [`master`](#master-branch).

## Issue

A feature of [Github](#github), which allows users to alert the owners of a [repository](#repository) of bugs and request features.

See the [Issues Tutorial](Tutorials/Issues.md) for more information.

## Local

Whenever you work on a repository on your machine, you are working on a _local copy_ of the repository. In order to make changes to the [remote](#remote) copy of the [repository](#repository), you will have to [commit](#commit) your changes to a [branch](#branch), and either [push](#push) your branch to the remote repository (in the case that you have privileges to do so) or submit a [pull request](#pull-request) to the owner of the remote repository (in the case that you do not).

## Markdown

Markdown is a lightweight text styling syntax which makes it easy to add basic **_styling_** to a plain text document.

This document is written in Markdown.

See the [Markdown Tutorial](Tutorials/Markdown.md) for more information.

## Master (Branch)

When you [create](#init) a [repository](#repository), a single [branch](#branch) is created which is called `master`.

_N.B.: You can rename / change your primary branch to something other than `master` if it feels more appropriate._

## Merge

One can merge the [commits](#commit) of one [branch](#branch) into another.

This may not always be trivial. For example, if there have been conflicting changes to a single line in a file, a [merge conflict](#merge-conflict) will be created, which must be resolved.

## Merge Conflict

If there are conflicting changes made to a single line in a file between one [commit](#commit) and another, a merge conflict is created, which must be resolved.

[Git](#git) will inject text like this:

	<<<<<<< HEAD
	The changes made to this line on the current branch
	=======
	Other changes made to this line on a different branch which conflict
	>>>>>>> other-branch
	
Sometimes Github will allow you to resolve these conflicts in the browser, but sometimes it is too complicated, and the changes must be [pulled](#pull) down and fixed manually.

## Organization

A Github feature which allows multiple users to collaborate on a given [repository](#repository) with varying scopes of privilege.

## Origin

When one [clones](#clone) a [remote](#remote) [repository](#repository), the remote repository will be named `origin`.

When updating this remote repository with changes from your [local](#local) copy, you may run the following command:

	git push origin branch-name
	
Here, you are [pushing](#push) your [commits](#commit) from your local copy of the repository to the remote copy of the repository, which is named `origin`. You may find yourself working on a project for which the remote is not named `origin`, and in that case, replace `origin` above with the appropriate name.

## PR

Short for [Pull Request](#pull-request).

## Pull

Bring down the changes made on a [remote](#remote) copy of a repository to your [local](#local) copy of the repository.

For example, in order to update your local copy of a repository on Github on the [`master`](#master) branch, you can use the following command:

	git push origin master

## Pull Request

A proposed change to a repository. A pull request represents the difference between one [branch](#branch) and another. When creating a pull request, you supply a title and a message. Once you create a pull request, you can still add [commits](#commit) to the [branch](#branch), and they will show up while the pull request is open.

Pull requests are helpful because Github elevates this process to become a venue for discourse around a given change. Even a small change in code could drastically alter the way a project behaves, and thus it may require a great deal of discussion before it can be considered worthy of [merging](#merge).

## Push

To upload the changes made on a [local](#local) copy of a [repository](#repository) to a [remote](#remote) repository, you can push.

For example, in order to update a repository on Github with the changes that you have made locally on the [`master`](#master) branch, you can use the following command:

	git push origin master

## Remote

In order to contribute to a [repository](#repository) served from [Github](#github), you must [clone](#clone) the repository to make a [local](#local) copy. The Github-served copy of the repository is considered a remote copy, and will be named `origin` by default.

You may find yourself collaborating with multiple people where they each have their own [forks](#fork) of the repository, and you may interact with each of these different repositories as remotes.

## Repo

Short for [Repository](#repository).

## Repository

A directory which whose changes are tracked by [Git](#git).