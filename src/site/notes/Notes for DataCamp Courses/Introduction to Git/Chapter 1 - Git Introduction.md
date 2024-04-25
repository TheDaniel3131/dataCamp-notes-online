---
{"dg-publish":true,"permalink":"/notes-for-data-camp-courses/introduction-to-git/chapter-1-git-introduction/","noteIcon":"","created":"2024-04-25T23:14:32.430+08:00","updated":"2024-04-25T23:33:05.408+08:00"}
---

# Introduction to version control with Git

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

Super shell skills! Being able to navigate directories and interact with files is extremely beneficial as you begin to work with Git.