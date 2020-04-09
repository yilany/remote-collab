# Configuring Git

Once you have [Git installed](InstallGit.md) on your computer, you have the ability to create and modify repositories locally. You can provide Git with your information so that you can automatically tag your commits with your name and email.

## Table of Contents

0. [Prereqs](#prereqs)
1. [Configure Your Identity](#configure-your-identity)

## Prereqs

- Basic comfort [getting around in the shell](GettingAroundShell.md)
- [Git installed](InstallGit.md)
- A [Github account](https://github.com)

## Configure Your Identity

Run the following command to tell Git what your name is, replacing "Jane Doe" with your own name:

	git config --global user.name "Jane Doe"
	
Check your work by running the following command:

	git config --global user.name
	
Then, run the following command to tell Git what your email is, replacing "jane.doe@example.com" with your own email address:

	git config --global user.email "jane.doe@example.com"
	
Check your work by running the following command:

	git config --global user.email
	
_You are not submitting this information to anyone! This is stored locally on your computer, and is used to tag your Git commits with your information. It is very helpful to have this information associated with your work, so that if you do share your work, someone can contact you if there is a problem or if they want to work with you._