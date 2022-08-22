# Git Cheatsheet

The following pages contains some useful info and commands to help you get the most out of Git:

* As a simple starting point I have found that GitLab's version of a [CheatSheet](https://about.gitlab.com/images/press/git-cheat-sheet.pdf)is easy to understand.
* For a full Git reference see this [Git SCM Book](https://git-scm.com/book/en/v2).

## Troubleshooting Git Issues

As with any tool you can sometimes run into issues, this section covers specific areas that I have come accross and how I went about solving these


### Git Case sensitivity or capitalisation

if you are moving files between different operating systems; sometime you can run into an issue where git is not case aware e.g. file name is 'Example' where you want to use 'example'.  whilst you may rename these files locally in your dev environment, however when you commit these changes into git it does not seem to recognise the issue.  To solve this you can simply:

1. ensure you are in your local git directory
1. run the 'git rm -r --cached . ' command to remove ALL local cache from this directory.
1. then re-add all files using the 'git add .' command
1. continue as normal by committing your changes.