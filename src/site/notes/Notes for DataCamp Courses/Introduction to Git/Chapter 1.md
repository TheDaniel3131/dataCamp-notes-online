---
{"dg-publish":true,"permalink":"/notes-for-data-camp-courses/introduction-to-git/chapter-1/","noteIcon":"","created":"2024-04-25T23:14:32.430+08:00","updated":"2024-04-26T11:31:31.469+08:00"}
---

# Introduction to version control with Git

# Lesson 1 - Git Introduction
## 1. Introduction to version control with Git

00:00 - 00:07

Hi! My name is George, and in this course we'll learn how to use Git for version control.

## 2. What is a version?

00:07 - 00:27

Before we discuss Git and version control, let's define a version, which is the contents of a file at a given point in time. It also includes metadata, or information associated with the file, such as the author, where it is located, the file type, and when it was last saved.

## 3. What is version control?

00:27 - 00:45

Version control is a group of systems and processes to manage changes made to documents, programs, and directories. Version control isn't just for software. Anything that changes over time or needs to be shared can benefit from using version control.

1. 1 Image credit: https://unsplash.com/@cdr6934

## 4. What is version control?

00:45 - 01:04

Version control allows us to track files in different states and let multiple people work on the same files simultaneously, a concept known as continuous development. It also allows us to combine different versions, identify a particular version of a file, and revert changes.

## 5. Why is version control important?

01:04 - 01:26

To illustrate why version control is essential when working with data, consider a common scenario of modifying a dataset. We save separate copies at various time intervals, using fairly similar names. We then produce new analyses as the dataset changes, but matching these outputs to the correct data can be difficult as time goes by!

## 6. Why is version control important?

01:26 - 01:37

Put another way, a data project without version control is like cooking without a recipe - it'll be difficult to remember how to produce the same results again.

1. 1 Image credit: https://unsplash.com/@mvdheuvel

## 7. Git

01:37 - 02:01

One popular program for version control is called Git. Git is open source and scalable to easily track everything from small solo projects to complex collaborative efforts with large teams! Note that Git is not the same as GitHub, which is a cloud-based Git repository hosting platform. However, it's common to use Git with GitHub!

## 8. Benefits of Git

02:01 - 02:22

A key benefit of Git is that it stores everything, so nothing is ever lost. Also, Git automatically notifies us when our work conflicts with someone else's, so it's harder to accidentally overwrite content. Additionally, Git can synchronize work done by different people on different machines.

## 9. Using Git

02:22 - 02:49

A common method to use Git is via the shell, also known as the terminal. The shell is a program for executing commands. Before we use Git, we'll run through some shell commands that will often be used in our version control workflow, such as previewing, modifying, and inspecting files or directories. Note that a directory is often referred to on a computer as a folder.

## 10. Useful shell commands

02:49 - 03:14

To see our location, we can execute pwd, which stands for print working directory. Here, we are in the Documents directory of a user called Repl. To see what is in our current directory we can use the ls command. This returns a list of all files and directories. There is a directory called archive and three csv files.

## 11. Changing directory

03:14 - 03:29

If we need to change directory, we can execute cd followed by the directory we want to move into. Here, we navigate to the archive directory. Rechecking our location confirms we have successfully moved.

## 12. Editing a file

03:29 - 03:52

We can even use the shell to preview and modify files. In the documents directory, we use the nano command followed by the filename, which opens a text editor. We can delete, add, or change contents of a file, and save using control and o, then exit the editor using control and x to return to the shell.

## 13. Editing a file

03:52 - 04:10

We can also use echo to create or edit a file. Here, we create a file called todo-dot-txt with a reminder to review our data for duplicates. If the file already exists, then we can append content by using two arrows instead of one.

## 14. Checking Git version

04:10 - 04:22

Different versions of software have different functionality, and Git is no exception. We can check which version of Git we have installed by typing git dash-dash-version in the shell.

## 15. Let's practice!

04:22 - 04:26

Now let's check our understanding of version control!


![Pasted image 20240425233254.png](/img/user/Pasted%20image%2020240425233254.png)

Super shell skills! Being able to navigate directories and interact with files is extremely beneficial as you begin to work with Git

![Pasted image 20240425233445.png](/img/user/Pasted%20image%2020240425233445.png)

Great work! The `--version` flag allows you to check what version of Git is installed locally, which is useful if you upgrade, or need to compare versions among colleagues.

# Lesson 2 - Saving files

## 1. Saving files

00:00 - 00:08

Now let's explore how Git stores information, along with looking at a workflow to update files and check their status.

## 2. A repository

00:08 - 00:18

To start, let's discuss the components of a Git project. We'll be working with a project about mental health in tech throughout the course, which is shown here.

## 3. A repository

00:18 - 00:31

There are two parts - the first is the files and directories that we create and edit, in this case a funding document, a markdown file containing a report, and a directory called data.

## 4. A repository

00:31 - 01:00

The second part is the extra information that Git records about the project's history. The combination of these two things is called a repository, often referred to as a repo. Git stores all of its extra information in a directory called dot-git, located in the main directory of the repo. Git expects this information to be laid out in a particular way, so we should not edit or delete dot-git.

## 5. Staging and committing

01:00 - 01:12

Now let's discuss how to make changes in a repo. We save a draft by placing it in a staging area. We save files, and update the repo in the process, through a commit.

1. 1 Image credits: https://unsplash.com/@brandomakesbranding; https://unsplash.com/@almapapi

## 6. Staging and committing

01:12 - 01:29

Putting files in the staging area is like placing a letter in an envelope, while making a commit is like putting the envelope in a mailbox. We can add more things to the envelope or take things out as often as we want, but once we put it in the mailbox we can't make further changes.

## 7. Accessing the .git directory

01:29 - 01:55

Although we shouldn't edit the dot-git directory, it may be helpful to see what's inside. It won't display when using the shell ls command, as it's a hidden directory. A hidden directory is a directory not displayed to users, typically because it stores information to enable programs to run. But if we add the dash-a flag it shows up along with some hidden files!

## 8. Making changes to files

01:55 - 02:20

Let's visualize the Git storage workflow. Here, we modify a markdown file called report-dot-md, and store five draft updates to the staging area as we progress. We commit, or save, the second and fifth versions of the file in the staging area, and with each commit our dot-git directory is modified to reflect the state of the repo.

## 9. Git workflow

02:20 - 02:30

So, our Git workflow is to modify a file, save the draft to the staging area, commit the updated file to our repo, and repeat!

## 10. Modifying a file

02:30 - 02:43

To execute this workflow we can use nano to open a text editor for the report file. We add three lines of text and save it using control-O and control-X.

## 11. Saving a file

02:43 - 03:01

To add the updated file to the staging area we use the command git add followed by the filename. Alternatively, we can add all modified files in the current directory using git add dot, as a dot represents all files and directories in our current location.

## 12. Making a commit

03:01 - 03:20

We then commit our drafts using git commit. We add the dash-m flag to allow us to include a log message about our commit, placing it in quotes. The log message is important as we can refer to it later. Best practice is to keep it short and concise.

## 13. Check the status of files

03:20 - 03:42

If we are making lots of changes then it's useful to know the status of our repo. We can use the git status command, which tells us which files are in the staging area, and which files have changes that aren't in the staging area yet. In this case, we see report-dot-md has been modified and is in the staging area, so we make a commit.

## 14. Let's practice!

03:42 - 03:45

Let's modify some files

![Pasted image 20240425233639.png](/img/user/Pasted%20image%2020240425233639.png)

Yes—all of the information about a repo is stored under its main directory, `mh_survey`.

![Pasted image 20240425233745.png](/img/user/Pasted%20image%2020240425233745.png)

Excellent! These commands are used extensively when performing version control in the Shell, so they are worth remembering!

![Pasted image 20240425234109.png](/img/user/Pasted%20image%2020240425234109.png)

Great Git skills! In three commands you've added a new row of data to a file, stored it as a draft, and made a commit to update the repo!

![Pasted image 20240426110713.png](/img/user/Pasted%20image%2020240426110713.png)

`git status` is a great way to see where you are in the version control workflow, allowing you to take steps to ensure everything is up-to-date. The commit output shows that two files were changed!

# Lesson 3 - Comparing Files

## 1. Comparing files

00:00 - 00:00

We've seen the workflow for drafting and saving updates, but if we are making lots of changes we need a way to compare versions as we make modifications!

## 2. Why compare files?

00:00 - 00:00

Perhaps we've made changes to a machine learning model, but we're getting poorer performance as a result. We want to revert our changes, but can't remember what the code for the model looked like previously.

1. 1 Image credit: https://unsplash.com/@mluotio83

## 3. Comparing a single file

00:00 - 00:00

Luckily, Git provides commands for checking the current state of our files versus at other times. Suppose we want to edit the report-dot-md file. Inside the text editor, we add two lines representing tasks to complete.

## 4. Updating the file

00:00 - 00:00

We've only edited one file, so we can use git add dot to add the report to the staging area. We then commit our changes.

## 5. Updating the file again

00:00 - 00:00

A while later we need to update the file again, this time removing the executive summary task and adding a reminder to cite the funding source. We can compare the last committed version of a file with the unstaged version by using the git diff command followed by the filename.

## 6. Comparing an unstaged file with the last commit

00:00 - 00:00

The output shows two versions of report-dot-md, where a is the first version, or the last one to be saved, and b is the second, or the one we have not added to the staging area.

## 7. Comparing an unstaged file with the last commit

00:00 - 00:00

The line with the two at symbols tells us the location of the changes, where the pairs of numbers represent the start line and number of lines. The minus one and five shows one line was removed at line five, and the plus one and five shows one line was added back in at line five.

## 8. Comparing an unstaged file with the last commit

00:00 - 00:00

Lines starting with a minus symbol written in red have been removed, the executive summary line in this case,

## 9. Comparing an unstaged file with the last commit

00:00 - 00:00

and lines starting with a plus symbol and written in green have been added - which is the last one.

## 10. Comparing a staged file with the last commit

00:00 - 00:00

What if we had already added the file to the staging area? We can use the git diff command again, but this time we add the dash-r flag to indicate we want to look at a particular revision of the file. Adding HEAD, which is a shortcut for the most recent commit, allows us to see a difference between the report file in the staging area and the version in the last commit. Note that the dash-r flag won't work if we don't put HEAD afterwards.

## 11. Comparing a staged file with the last commit

00:00 - 00:00

As we can see, the output gives us the same information as using git diff for a file that hasn't been added to the staging area!

## 12. Comparing multiple staged files with the last commit

00:00 - 00:00

What if we have more than one file in the staging area? Here we use cd to switch into the data directory, use nano to modify mh-tech-survey-dot-csv to add an extra participant's survey responses, then add the file to the staging area.

## 13. Comparing multiple staged files with the last commit

00:00 - 00:00

In this case, we can use git diff dash-r HEAD to show the difference between all files in the staging area. In the output, we can see two files have been modified. One new line was added to the end of the mh-tech-survey-dot-csv file, shown in green, along with the two changes to the report.

## 14. Recap

00:00 - 00:00

To recap, if we want to compare an unstaged file with the last commit we use git diff filename. To see a staged file versus the last commit we run git diff dash-r HEAD filename. For comparing all staged files with the last commit it's git diff dash-r HEAD.

## 15. Let's practice!

00:00 - 00:00

Now let's use Git to compare the difference between files at different times.

![Pasted image 20240426112716.png](/img/user/Pasted%20image%2020240426112716.png)

Yes— the `git diff` output shows three lines changed at line 48 in the last commit, and one additional line has been added in our current unstaged file.

![Pasted image 20240426113005.png](/img/user/Pasted%20image%2020240426113005.png)

Great work—in three steps you compared all files to their last committed version, and updated `report.md`!

![Pasted image 20240426113125.png](/img/user/Pasted%20image%2020240426113125.png)

Great work, looks like a reminder to update the analysis was added! In the next chapter, we will discover some of Git's more advanced functionality including the metadata it stores, how to look at versions from specific commits, and how to undo changes!

