---
{"dg-publish":true,"permalink":"/notes-for-data-camp-courses/introduction-to-git/chapter-4/","noteIcon":"","created":"2024-04-26T15:33:00.871+08:00","updated":"2024-04-26T15:49:54.580+08:00"}
---

# Lesson 1 - Creating repos

## 1. Creating repos

00:00 - 00:00

We know how to work with pre-existing Git repos, so let's look at how we can make new repos, and convert an existing project into a Git repo.

## 2. Why make a repo?

00:00 - 00:00

There are many benefits to creating a Git repo, which we've previously highlighted. To recap, the main reasons include the ability to systematically track the versions of files, to provide an easy way to collaborate with colleagues, and store everything so we can avoid losing our files!

1. 1 Image credit: https://unsplash.com/@jasongoodman_youxventures

## 3. Creating a new repo

00:00 - 00:00

Imagine we've secured funding for a project following up on our mental health in tech companies project, which will compare mental health in the workplace across a range of sectors. Here, we create a new Git repo for this project using the git init command, followed by the name of our project called mental-health-workspace. Git creates a new subdirectory in the directory we were located in when we ran the git init command, with the name we provided for the repo. We can use cd to change into this directory. We can check that the Git repo has initialized correctly by running git status. Success! The output confirms we have a Git repo, and that no commits have been made yet.

## 4. Converting a project

00:00 - 00:00

Now we know how to create a Git repo from scratch, let's look at how to convert an existing project into a repo. Let's say we started working on our new mental health project without first creating a new Git repo. We can convert the directory to a Git repo by executing git init. We run the command from our project directory, and Git confirms that an empty repo has been created along with providing the location.

## 5. What is being tracked?

00:00 - 00:00

Something interesting happens if we check the status of the repo. We can see Git has immediately recognized that there are modified files, in this case, the report-dot-md file, so we are encouraged to add our files to the staging area and make a commit!

## 6. Nested repositories

00:00 - 00:00

One word of caution when creating Git repos. We should avoid creating a Git repo inside another Git repo, also known as nested repos. If we do this, there will be two dot-git directories. Unfortunately, as we try to make commits, Git will get confused about which directory it needs to update. Generally, nested repos are not necessary except when working on extremely large and complex data projects!

## 7. Let's practice!

00:00 - 00:00

Time to make our own Git repos!

![Pasted image 20240426153451.png](/img/user/Pasted%20image%2020240426153451.png)

Impressive initialization—in just three lines of code you created a new Git repository, moved into its main directory, and created a to-do list!

![Pasted image 20240426153539.png](/img/user/Pasted%20image%2020240426153539.png)

Great work—by converting an existing project into a Git repos your files are now being tracked! Now let's learn about an essential component of working with Git—remote branches!

# Lesson 2 - Working with Remotes

## 1. Working with remotes

00:00 - 00:08

Now we're going to learn about a fundamental feature for collaboration in Git - remote repos, also known as remotes.

## 2. What is a remote?

00:08 - 00:19

When someone mentions a remote, we might think they're talking about a device used to control a television. However, in Git, a remote means something entirely different!

1. 1 Image credit: https://unsplash.com/@glenncarstenspeters

## 3. Local repo

00:19 - 00:33

So far, we have worked with repos stored on our computer. These are known as local repos. They are great if we are working on a local project, but what if we need to collaborate with colleagues? How will they access our repo?

## 4. Remote repo

00:33 - 00:43

This is where remotes solve our problems! A remote repo is a repo stored in the cloud through an online repo hosting service such as GitHub.

## 5. Why use remote repos?

00:43 - 01:00

There are a couple of key benefits to using remotes. If our computer breaks down or we lose it, we can use a different computer to access our project from the remote repo as it is backed up there! Additionally, colleagues can collaborate with us regardless of their location.

1. 1 Image credit: https://unsplash.com/@mahlkornel

## 6. Cloning locally

01:00 - 01:28

We can copy existing remotes to our local computer by cloning them. If required, we can also clone a local repo. To do this we use the git clone command followed by the path to the project directory. Here, we clone a local project from home-slash-john-slash-repo. We can also give the cloned repo a name by specifying it after the path, such as here, where we call it new-repo.

## 7. Cloning a remote

01:28 - 02:00

While remotes can exist locally, it is more common to store them in an online repo hosting service such as GitHub, Bitbucket, or Gitlab. If we have a GitHub account then we can access a remote stored on their server by cloning it on to our local computer. To do this we again use the git clone command, this time providing a URL rather than a local path. For example, here we clone a repo from github-dot-com-slash-datacamp-slash-project.

## 8. Identifying a remote

02:00 - 02:19

When we clone a repo, Git remembers where the original repo was. It does this by storing a remote tag in the new repo's configuration. If we are in a repo, we can list the names of its remotes using git remote. The output confirms we have cloned the datacamp GitHub project.

## 9. Getting more information

02:19 - 02:38

If we want more information, such as the remotes URLs, we can add the dash-v flag, which stands for verbose. We see two outputs. They contain the same URL, but have either fetch or pull at the end of their respective rows. We will discuss these terms later in the chapter.

## 10. Creating a remote

02:38 - 03:16

When cloning, Git will automatically name the remote as origin. We can add more remotes by specifying a name for Git to assign. We do this using the git remote add command, and provide two pieces of information - the name that we would like to assign to the remote repo, and the URL, or the path to the directory. Here, we create a remote called george, which points to the url github-dot-com-slash-george-underscore-datacamp-slash-repo. It is useful to define the remote name as we can use it as a shortcut when merging rather than listing the URL or path.

## 11. Let's practice!

03:16 - 03:21

Now it's time to practice working with remotes!

![Pasted image 20240426153755.png](/img/user/Pasted%20image%2020240426153755.png)

Awesome! `git clone` is a very useful command for copying other repos onto your local computer, whether from another local directory or remote storage such as GitHub. Now you can build on the work John has done so far!

![Pasted image 20240426154157.png](/img/user/Pasted%20image%2020240426154157.png)

Adding the name `john` will save you time when accessing or merging the cloned repo! Now let's learn how to keep files in sync between local and remote branches.

# Lesson 3 - Gathering from a remote

## 1. Gathering from a remote

00:00 - 00:07

We've seen how to clone remote repos, now let's look at how to get content from a remote into our local repo.

## 2. Remote vs. local

00:07 - 00:22

Say we have been working in a branch of our local repo, but others have been working in the remote. Here, we can see the contents of the two repos, and it is clear that there are additional files and subdirectories in the remote.

## 3. Collaborating on Git projects

00:22 - 00:44

If several people are collaborating on a project then, in practice, they will access the remote, work on files locally, save them, and synchronize their changes between the remote and local repos. This means that the remote repo should be the source of truth for the project, where the latest versions of files that are not drafts can be located.

## 4. Fetching from a remote

00:44 - 01:10

To compare the files in a remote against the contents of a local repo we first need to fetch versions from the remote. We do this using the git fetch command, providing the name of the remote, and the local branch to fetch into. Here we fetch from the origin remote. The output shows us the URL or path we are fetching from, the branch, which is main, and that we are fetching the HEAD, or last commit.

## 5. Fetching from a remote

01:10 - 01:20

If we want to fetch into a different branch, we specify it. For example, here, we fetch from the remote origin repo's report branch.

## 6. Synchronizing content

01:20 - 02:01

After fetching, we now have the contents of the remote in our local repo. However, we need to synchronize contents between the two repos. To do this, we perform a merge of the remote into the local repo's main branch, where we are currently located. The output shows the two commit hashes, followed by the type of merge. In this case it is a fast-forward, meaning the local repo was behind the remote, and this merge aligned it. We see two files were changed, mental-health-survey-dot-csv had three lines added, and report-dot-md had one line added. The last line summarizes the changes.

## 7. Pulling from a remote

02:01 - 02:29

As the remote is the source of truth, it is often ahead of local repos, meaning the workflow of fetching content and synchronizing locally is very common. To simplify this process, Git allows us to fetch and merge using a single command. We execute git pull followed by the remote repo's name and the local repo branch we are merging into. Here, we pull from origin into our local main branch.

## 8. Pulling from a remote

02:29 - 02:40

The output confirms this is a combination of the two commands, with the git fetch output shown in the first two lines, and the git merge output displayed in the remaining five lines!

## 9. Pulling with unsaved local changes

02:40 - 03:09

If we have been working locally and not yet committed our changes, then Git won't allow us to pull from a remote. Let's say we've added a new line to the report but not staged the file or made a commit. If we try to pull from origin then Git tells us that local changes would be overwritten. We are instructed to commit our changes and told that the pull command was aborted. Therefore, it's important to save our work locally before we pull from a remote.

## 10. Let's practice!

03:09 - 03:14

Time to practice fetching and pulling in Git!

![Pasted image 20240426154403.png](/img/user/Pasted%20image%2020240426154403.png)

Fantastic fetching! Looks like John added a reminder about references in `report.md`, as the local `main` branch doesn't have this content in the file.

![Pasted image 20240426154536.png](/img/user/Pasted%20image%2020240426154536.png)

Perfect pulling! Notice you received the output `1 file changed, 1 insertion(+)`, highlighting that the remote was ahead of your local repo!

# Lesson 4 - Pushing to a remote

## 1. Pushing to a remote

00:00 - 00:08

We've seen how to bring our local branch up to date with a remote repo, but what about bringing our local changes into a remote repo?

## 2. Pulling from a remote

00:08 - 00:15

To recap, we use git pull to gather content from a remote and merge into our local repo.

## 3. Pushing to a remote

00:15 - 00:26

The opposite of this task is merging content from a local repo into a remote. Therefore, the opposite of pulling means that we push our changes to the remote.

## 4. git push

00:26 - 01:02

As with pulling contents from a remote, we need to commit local changes before we can push to the remote. Once we have done this, we can push to a remote using the git push command, supplying two arguments. First we provide the remote, followed by the local branch. The order that we supply the remote repo and the local branch is the same as git pull. So, we can think of it as pushing content into the remote repo from the local branch. Here, we push changes into origin from our local main branch.

## 5. Push/pull workflow

01:02 - 01:10

The typical push/pull workflow is as follows. We start by pulling the remote into our local repo.

## 6. Push/pull workflow

01:10 - 01:15

We then work on our project locally, committing changes as we go.

## 7. Push/pull workflow

01:15 - 01:24

Lastly, we push our updated local repo to the remote. This workflow is repeated throughout our time working on the project.

## 8. Pushing first

01:24 - 01:34

What happens if we don't start the workflow by pulling from the remote? Here, we try to push the contents of our local repo's main branch to the remote.

## 9. Remote/local conflicts

01:34 - 01:37

Git gives us a large output! Let's break it down.

## 10. Remote/local conflicts

01:37 - 01:42

The first line shows us the remote repo URL we are trying to push to.

## 11. Remote/local conflicts

01:42 - 01:48

The second and third lines show us the outcome of the command - it was rejected and failed.

## 12. Remote/local conflicts

01:48 - 02:27

In the third to seventh lines, Git provides hints. This is where Git tells us why the command failed, and recommends what we should do to resolve the issue. In this case, we see that the tip, or the end, of our current branch is behind its remote counterpart and the suggestion is to pull from the remote before trying to push our local changes again. This can typically occur because while we've been working locally, our colleagues have been pushing their changes to the remote. So, if we don't pull from the remote at the start of the workflow then our local repo won't be synchronized with the remote.

## 13. Resolving a conflict

02:27 - 02:59

Previously we saw that git pull used a fast-forward merge. In this case it's slightly different, as there are different commits on the local and remote repos, so Git can't just bring them in line with one another. So, when we try to pull, Git will automatically open the nano text editor and ask us to add a message for the merge. We leave a message that we are pulling the latest report from the remote. We use Control and O to save, then Control and X to exit as usual.

## 14. Avoid leaving a message

02:59 - 03:08

We can avoid providing a message by including dash-dash-no-edit when executing git pull, however, this is not recommended!

## 15. Resolving a conflict

03:08 - 03:27

After saving our message, we see that the merge has been made using a recursive strategy, and report-dot-md was updated. When using a Git version between zero-point-nine-nine-point-nine and two-point-three-three-point-zero, this is the default merge strategy.

## 16. Pushing to the remote

03:27 - 03:48

As this change has now been incorporated locally, we can try to push our changes again. The output provides a lot of information, but the key takeaway is that the changes have been written to the remote repo. The final line shows the commit hashes referenced for merging the local repos's main branch into the remote's main branch.

## 17. Let's practice!

03:48 - 03:55

Let's push things with some exercises to synchronize our local and remote repos!

![Pasted image 20240426154829.png](/img/user/Pasted%20image%2020240426154829.png)

Now you know how to pull changes from a remote, work locally, and push your changes back to the remote! But what happens if the remote is ahead of the local repo?

![Pasted image 20240426154915.png](/img/user/Pasted%20image%2020240426154915.png)

Excellent—you've learned how to use `git push` and `git pull` to deal with a remote repo that has different content to your local repo. Let's quickly recap on what we've covered in the course!

# Congratulations!

## 1. Congratulations!

00:00 - 00:02

Great work on completing the course!

## 2. What you've covered

00:02 - 00:14

You've come a long way, starting with the definition of a version, discovering why version control is important for data projects, and learning how to use Git for saving and comparing files.

## 3. What you've covered

00:14 - 00:20

You progressed into understanding how Git stores data and interpreting the commit structure,

## 4. What you've covered

00:20 - 00:25

as well as applying the fundamental skills of undoing and reverting changes.

## 5. What you've covered

00:25 - 00:35

You configured settings to speed up your workflow, such as creating an alias for a common command, and worked across multiple branches.

## 6. What you've covered

00:35 - 00:40

You also saw how to recognize Git's conflict syntax to handle merge conflicts!

## 7. What you've covered

00:40 - 00:50

Lastly, you learned how to clone and synchronize content across local and remote repos - a fundamental skill for collaboration!

## 8. Git cheat sheet

00:50 - 01:08

Version control with Git involves a lot of complex commands, which seasoned Git users can often forget. So don't be afraid to refer back to this course for commands and concepts you need a refresher on, or you can refer to our cheat sheet available at this link!

## 9. Thank you!

01:08 - 01:17

Thanks again for taking the course. Hopefully you now feel equipped to implement version control with Git in your future projects!

- [  
    ](https://www.datacamp.com/courses/29712/chapters/98679/continue)