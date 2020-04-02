# Modifying Contents in the Shell

## Table of Contents

0. [Prereqs](#prereqs)
1. [Create a Directory (`mkdir`)](#create-a-directory-mkdir)
2. [Create a File (`touch`)](#create-a-file-touch)
3. [Remote Contents (`rm`)](#remove-contents-rm)

## Prereqs

- You are reading this on a computer with a keyboard of some sort
- You have the `Terminal` application or an equivalent command line interface installed
- You know the [basics of getting around in the shell](GettingAroundShell.md)

## Create a Directory (`mkdir`)

[Navigate to a directory of your choosing](GettingAroundShell.md), and run the following command:

	mkdir TigerKingResearch

Now, run the `ls` command and your new directory should show up. Feel free to `cd` into your new directory and `cd ..` back up to where you are now.

_For more information, run the `man mkdir` command to see the manual documentation for the `touch` command. Press `q` to escape the `less` program!_

## Create a File (`touch`)

`cd` into your new directory (ours is called `TigerKingResearch`), and we will create a new [Markdown](Markdown.md) file to start your independent investigation:

	touch WhereIsDon.md
	
The `touch` command creates an empty file with the given name (and much more beyond the scope of this tutorial).

_For more information, run the `man touch` command to see the manual documentation for the `touch` command. Press `q` to escape the `less` program!_

## Remove Contents (`rm`)

### Remove a File (`rm`)

After you travel to Costa Rica and back a few times, maybe your investigation into Jack Donald "Don" Lewis' whereabouts drags you into some scary territory, and you need to delete the artifacts of your research.

We can run the "remove directory entries" command to get rid of it:

	rm WhereIsDon.md
	
Now, run `ls` to make sure there is no trace of your research.

### Remove a Directory (`rm -r`)

To be even more sure that you cover your tracks, let's remove the `TigerKingResearch` directory altogether. First, `cd ..` up to the directory containing your `TigerKingResearch` directory, and run the `ls` command to make sure that you are in the right place.

If you try to run the following command:

	rm TigerKingResearch
	
You will see the following error:

	rm: TigerKingResearch: is a directory
	
Because we are working with a directory rather than a file, we need to remove our directory _recursively_. Try this command instead:

	rm -r TigerKingResearch
	
Run the `ls` command to make sure the `TigerKingResearch` is deleted for good. You should be in the clear.

_For more information, run the `man rm` command to see the manual documentation for the `rm` command. Press `q` to escape the `less` program!_

⚠️ **You are walking into dangerous territory here with the `rm` command**. If you are not careful, you can inadvertently delete important files with no way of undoing your mistake. Even the pros make this mistake: see how [90% of Toy Story 2 was accidentally deleted using the `rm -rf *` command](https://thenextweb.com/media/2012/05/21/how-pixars-toy-story-2-was-deleted-twice-once-by-technology-and-again-for-its-own-good/).

