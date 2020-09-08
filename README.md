# cs302-F2020-lab1-starter

![](../../workflows/build/badge.svg)

## Table of Contents

* [Table of Contents](#table-of-contents)
* [Objectives](#objectives)
* [Introduction](#introduction)
* [Continuous Learning](#continuous-learning)
* [Assignment Reminders](#assignment-reminders)
* [Configuring Git and GitHub](#configuring-git-and-github)
* [Accessing the Assignment](#accessing-the-assignment)
* [Laboratory Assignment Tasks](#laboratory-assignment-tasks)
  + [Unscrambling the Markdown File](#unscrambling-the-markdown-file)
  + [Running a Web Server](#running-a-web-server)
  + [Interacting with Remote Servers](#interacting-with-remote-servers)
  + [Reflecting on the Laboratory Assignment](#reflecting-on-the-laboratory-assignment)
* [Automated Checks with GatorGrader](#automated-checks-with-gatorgrader)
* [Assignment Assessment](#assignment-assessment)
* [Advance Feedback on an Assignment](#advance-feedback-on-an-assignment)
* [Discussion of a Graded Assignment](#discussion-of-a-graded-assignment)
* [Additional Resources](#additional-resources)
  + [System Commands](#system-commands)
  + [Using Docker](#using-docker)
  + [Using the Docker Shell](#using-the-docker-shell)
  + [Downloading Project Updates](#downloading-project-updates)
  + [Using GitHub Actions](#using-github-actions)
  + [System Requirements](#system-requirements)
  + [Reporting Problems](#reporting-problems)
  + [Receiving Assistance](#receiving-assistance)

## Objectives

The learning objectives for this laboratory assignment are as follows:

- To configure Git and GitHub on your laptop and on the GitHub servers
- To transfer files from your laptop to your GitHub repository
- To use your text editor to manipulate code blocks in a Markdown file
- To use a Docker container to run the automated checks performed by GatorGrader
- To use a terminal window to run a web server through a Python program and observe its output
- To learn how to interpret the output of networking programs like [dig](https://en.wikipedia.org/wiki/Dig_(command)) and [mtr](http://www.bitwizard.nl/mtr/)

## Introduction

Designed for use with [GitHub Classroom](https://classroom.github.com/) and
[GatorGrader](https://github.com/GatorEducator/gatorgrader/), this repository
contains a laboratory assignment for a web development course. The source code
and technical writing for this assignment must pass tests set by the
[GatorGrader tool](https://github.com/GatorEducator/gatorgrader). When you use
the `git commit` command to transfer your source code to your GitHub
repository, GitHub Actions will initialize a build of your assignment, checking
to see if it meets all of the requirements. If both your source code and
writing meet all of the established requirements, then you will see a green ✔
in the listing of commits in GitHub. If your submission does not meet the
requirements, a red ❌ will appear instead. Please note that, at the option of
the course instructor, some checks may be run in GitHub Actions that are not
run locally by the [GatorGrader
tool](https://github.com/GatorEducator/gatorgrader).

## Continuous Learning

If you have not done so already, please read all of the relevant [GitHub
Guides](https://guides.github.com/) that explain how to use many of the features
that GitHub provides. In particular, please make sure that you have read the
following GitHub guides: [Mastering
Markdown](https://guides.github.com/features/mastering-markdown/), [Hello
World](https://guides.github.com/activities/hello-world/), and [Documenting Your
Projects on GitHub](https://guides.github.com/features/wikis/). Each of these
guides will help you to understand how to use both [GitHub](http://github.com) and
[GitHub Classroom](https://classroom.github.com/).

Students who want to learn more about how to use
[Docker](https://www.docker.com) should review the [Docker
Documentation](https://docs.docker.com/). Students are also encouraged to
review the documentation for their text editor, which is available at [VS
Code](https://code.visualstudio.com/docs). You should also review the [Git
documentation](https://git-scm.com/doc) to learn more about how to use the Git
command-line client. In addition to talking with the instructor and technical
leader for your course, students are encouraged to search
[StackOverflow](https://stackoverflow.com/) for answers to their technical
questions.

As outlined in the course schedule in the [course planning
repository](https://github.com/Allegheny-Computer-Science-302-F2020/cs302-F2020-plans),
students should also read all of the assigned readings for up to and including
the week of the semester on which this laboratory assignment was assigned.

## Assignment Reminders

- **Follow each step carefully**. Slowly read each sentence in this document,
  making sure that you precisely follow each instruction. Take notes about each
  step that you attempt, recording your questions and ideas and the challenges
  that you faced. If you are stuck, then please tell a technical leader or the
  course instructor what assignment step you recently completed.

- **Regularly ask and answer questions**. Please log into Slack at the start of
  the laboratory session and then join the appropriate channel. If you have a
  question about one of the steps in an assignment, then you can post it to the
  designated channel, discussing your questions through both Slack and the
  Google Meet designated for the class.

- **Store your files in GitHub**. Starting with this laboratory assignment, you
  will be responsible for storing all of your files (e.g., Python source code
  and Markdown-based writing) in a Git repository using GitHub Classroom. Please
  verify that you have saved your source code in your Git repository by using
  `git status` to ensure that everything is updated. You can see if your
  assignment submission meets the established correctness requirements by using
  the provided checking tools on your local computer and by checking the commits
  in GitHub.

- **Keep all of your files**. Don't delete your programs, output files, and
  written reports after you submit them through GitHub; you will need them
  again when you study for the course assessments and work on the other
  laboratory, practical, and technical challenge assignments.

- **Hone your technical writing skills**. Computer science assignments require
  to you write technical documentation and descriptions of your experiences when
  completing each task. Take extra care to ensure that your writing is
  interesting and both grammatically and technically correct, remembering that
  computer scientists must effectively communicate and collaborate with their
  team members and the student technical leaders and course instructor.

- **Review the Honor Code on the syllabus**. While you may discuss your
  assignments with others, copying source code or technical writing is a
  violation of Allegheny College's Honor Code.

## Configuring Git and GitHub

During this laboratory assignment and the subsequent laboratory and practical
assignments, we will securely communicate with the GitHub servers that will host
all of the project templates and your submitted deliverables. In this
assignment, you will perform all of the steps to configure your account on
GitHub and you will start your first assignment using GitHub Classroom. As you
will be required to use Git, an industry standard tool, in all of the remaining
laboratory and practical assignments and during the class sessions, you should
keep a record of all of the steps that you complete and the challenges that you
face. You may chat with the course instructor or one of the technical leaders if
you are not able to complete a certain step or if you are not sure how to
proceed.

- If you do not already have a GitHub account, then please go to the GitHub web
  site and create one, making sure that you use your `allegheny.edu` email
  address so that you can join GitHub as a student at an accredited educational
  institution. You are also encouraged to sign up for GitHub's "Student
  Developer Pack" at [Student Developer
  Pack](https://education.github.com/pack), qualifying you to receive free
  software development tools. Additionally, please add a description of yourself
  and an appropriate professional photograph to your GitHub profile. Unless your
  username is taken, you should also pick your GitHub username to be the same as
  Allegheny's Google-based email account. Now, in the `#labs` channel of our
  Slack workspace, please type on one line your full name, `allegheny.edu` email
  address, and your new GitHub username.

- If you have never done so before, you must use the `ssh-keygen` program to
  create secure-shell keys that you can use to support your communication with
  GitHub. But, to start, this task requires you to type commands in a program
  that is known as a terminal. Your terminal program will vary depending on your
  operating system. For instance, if you are running Linux, you can click on an
  icon that contains the `>` symbol or press the "Super" key, start typing the
  word "terminal", and then select that program. Another way to open a terminal
  involves typing the key combination `<Ctrl>-<Alt>-t`. On the Windows operating
  system you may want to use the "Command Prompt" or the "Power Shell" and on
  MacOS you can use "Terminal". Your terminal will display as a box into which
  you can type commands. For the next step, you may need to separately install
  `ssh-keygen` if it is not on your laptop.

- Now that you have started the terminal, you will need to type the `ssh-keygen`
  command in it. Follow the prompts to create your keys and save them in the
  default directory. That is, you should press "Enter" after you are prompted to
  "`Enter file in which to save the key ...  :`" and then type your selected
  passphrase whenever you are prompted to do so. Please note that a "passphrase"
  is like a password that you will type when you need to prove your identify to
  GitHub. What files does "`ssh-keygen`" produce? Where does this program store
  these files by default? Do you have any questions about how to create your SSH
  keys?

- Once you have created your ssh keys, you need to upload them to GitHub. First,
  you must log into GitHub and look in the right corner for an account avatar
  with a down arrow. Click on this link and then select the "Settings" option.
  Now, scroll down until you find the "SSH and GPG keys" label on the left,
  click to create a "New SSH key", and then upload your ssh key to GitHub. You
  can copy your SSH key to the clipboard by going to the terminal and typing a
  command like `cat ~/.ssh/id_rsa.pub` command and then highlighting this
  output. When you are completing this step in your terminal, please make sure
  that you only highlight the letters and numbers in your key &mdash; if you
  highlight any extra symbols or spaces then this step may not work correctly.
  Then, paste this into the GitHub text field in your web browser.

- Again, when you are completing these steps, please make sure that you take
  careful notes about the inputs, outputs, and behavior of each command. If
  there is something that you do not understand, then please ask the course
  instructor or the technical leader about it.

- Since this is your first laboratory assignment and you are still learning how
  to use the appropriate software, don't become frustrated if you make a
  mistake. Instead, use your mistakes as an opportunity for learning both about
  the necessary technology and the background and expertise of the other
  students in the class, the technical leaders, and the course instructor.
  Remember, you can use Slack to talk with the instructor by typing `@gkapfham`
  in a channel.

## Accessing the Assignment

To access this assignment, you should go into the `#announcements` channel in
our Slack workspace and find the announcement that provides a link for it. Copy
this link and paste it into your web browser. Now, you should accept the
laboratory assignment and see that GitHub Classroom created a new GitHub
repository for you to access the assignment's starting materials and to store
the completed version of your assignment. Specifically, to access your new
GitHub repository for this assignment, please click the green "Accept" button
and then click the link that is prefaced with the label "Your assignment has
been created here". If you accepted the assignment and correctly followed these
steps, you should have created a GitHub repository with a name like
`Allegheny-Computer-Science-302-Fall-2020/computer-science-302-fall-2020-lab-1-gkapfham`.
Unless you provide the course instructor with documentation of the extenuating
circumstances that you are facing, not accepting the assignment means that you
automatically receive a failing grade for all of its components.

Before you move to the next step of this laboratory assignment, please make sure
that you read all of the content on the web site for your new GitHub repository,
paying close attention to the technical details about the commands that you will
type and the output that your program must produce. Now you are ready to
download the starting materials to your laboratory computer. Click the "Clone or
download" button and, after ensuring that you have selected "Clone with SSH",
please copy this command to your clipboard. At this point, you can open a new
terminal window and type the command `mkdir cs302F2020`. To enter into this
directory you should now type `cd cs302F2020`. Next, you can type the either
`ls` (on either MacOS or Linux) or `dir` (on Windows 10 Pro or Windows 10
Enterprise) and see that there are no files or directories inside of this
directory. By typing `git clone` in your terminal and then pasting in the string
that you copied from the GitHub site you will "download" all of the code for
this assignment. For instance, if the course instructor ran the `git clone`
command in the terminal, it would look like:

```
git clone git@github.com:Allegheny-Computer-Science-302-F2020/computer-science-302-fall-2020-lab-1-gkapfham.git
```

After this command finishes, you can use `cd` to change into the new directory.
If you want to "go back" one directory from your current location, then you can
type the command `cd ..`. Finally, please continue to use the `cd` and `ls`
commands to explore the files that you automatically downloaded from GitHub. If
one of the aforementioned commands does not work correctly, then it is possible
that your terminal window is not up-to-date or not configured correctly. In this
case, please share your specific error messages with the instructor, ultimately
working to master the use of terminal commands. What files and directories do
you see? What do you think is their purpose? Spend some time exploring, telling
your discoveries to a student technical leader.

## Laboratory Assignment Tasks

### Unscrambling the Markdown File

If you look in the `src/markdown/learning-objectives` directory you will see
that it contains the Markdown file that features the learning objectives for
this course. You can find the correct version of these files in the [Computer
Science 302 Course Planning
Repository](https://github.com/Allegheny-Computer-Science-302-F2020/cs302-F2020-plans).
If you carefully inspect this file in your text editor, you will find that it
is no longer in the correct order. Your task for this phase of the assignment
is to "unscramble" the content in this Markdown files so that it looks the
same as the content in the aforementioned course planning repository.

### Running a Web Server

Your GitHub repository contains an file called `web-development.html` in the
`src/html/learning-objectives`. Another way to see how the Markdown file from
the previous step should correctly render is to run a web server that points to
the directory containing this HTML file and then to load that server into your
web browser. Upon completing this step you should be able to see the correct
headers and lists that should be in the `web-development.md` file. Ultimately,
the rendered content of your `web-web-development.md` should match the rendered
content in the course planning repository and in your web browser as it views
the HTML from your server. Here is the command to type in your terminal window
for starting the HTTP server using the Python programming language on your
laptop:

```
python -m http.server --directory src/html/learning-objectives
```

When I look in my terminal window after accessing the file served by this HTTP
server I see the following output. Can you explain what this output means? What
output do you see in your terminal window?

```
127.0.0.1 - - [08/Sep/2020 13:26:54] "GET / HTTP/1.1" 200 -
127.0.0.1 - - [08/Sep/2020 13:26:56] "GET /web-development.html HTTP/1.1" 200 -
```

### Interacting with Remote Servers

Much like the debugging output that you produced by running the local
Python-based server in the previous step, there are many networking programs
like [dig](https://en.wikipedia.org/wiki/Dig_(command)) and
[mtr](http://www.bitwizard.nl/mtr/) that you can run to see how data flows from
your laptop to remote servers that are publicly accessible on the Internet. The
two programs that we are going to learn more about as part of this laboratory
assignment are called `dig` and `mtr`. You can install the `dig` program by
following the instructions in [this
article](https://help.dyn.com/how-to-use-binds-dig-tool/) and you can install
the `mtr` program by following the instructions in [this
article](https://help.distilnetworks.com/hc/en-us/articles/215640947-How-to-Run-an-MTR).
While all students should attempt to install this program, at minimum you need
to be able to interpret the output of these tools as given in the
`writing/reflection.md` file in your GitHub repository. For instance, here is
the output from running the command `mtr www.github.com` in the instructor's
terminal window. Using the material in Chapters 1 and 2 of the textbook, can you
interpret the meaning of the output from running `mtr`?

```
Keys:  Help   Display mode   Restart statistics   Order of fields   quit
                                   Packets               Pings
 Host                            Loss%   Snt   Last   Avg  Best  Wrst StDev
 1. _gateway                      0.0%     5    1.1   1.8   1.1   3.5   1.0
 2. dynamic-acs-72-23-183-1.zoom  0.0%     5    8.6  10.9   8.6  16.1   3.2
 3. 10.201.22.66                  0.0%     5   19.5  13.8  10.4  19.5   4.1
 4. 10.200.2.61                   0.0%     5   10.8  12.3   9.9  14.8   2.0
 5. 10.200.3.34                   0.0%     5   12.4  13.5  11.7  16.2   1.8
 6. 10.200.2.117                  0.0%     5   11.4  14.0  11.4  15.3   1.6
 7. ce-0-6-0-1.r01.nycmny17.us.b  0.0%     5   76.9  39.0  28.7  76.9  21.2
 8. ae-2.r21.nwrknj03.us.bb.gin. 20.0%     5   29.7  30.2  29.7  30.7   0.6
 9. ae-3.r25.asbnva02.us.bb.gin. 20.0%     5   36.0  42.7  33.9  64.8  14.8
10. ae-7.r06.asbnva02.us.bb.gin.  0.0%     5   35.1  53.4  35.1 121.0  37.9
11. ce-0-6-0-1.r06.asbnva02.us.c  0.0%     5   32.2  40.5  32.2  61.2  11.8
15. lb-140-82-112-4-iad.github.c  0.0%     4   33.2  32.0  30.5  33.2   1.2
```

### Reflecting on the Laboratory Assignment

Once you have finished both of the previous technical tasks, use your text
editor to answer all of the questions in the `writing/reflection.md` file. For
instance, you should explain the meaning of the three provided commands and
answer all of the other questions about your experiences in completing this
laboratory assignment.

## Automated Checks with GatorGrader

In addition to meeting all of the requirements outlined in this assignment
sheet, your submission must pass the following checks that
[GatorGrader](https://github.com/GatorEducator/gatorgrader) automatically
assesses:

If [GatorGrader's](https://github.com/GatorEducator/gatorgrader) automated
checks pass correctly, the tool will produce the output like the following in
addition to returning a zero exit code (which you can access by typing the
command `echo $?`). You will need to run
[GatorGrader](https://github.com/GatorEducator/gatorgrader) in a Docker
container by following the steps in the [Using Docker](#using-docker) section.

- The file reflection.md exists in the writing directory
- The file web-development.html exists in the src/html/learning-objectives directory
- The file web-development.md exists in the src/markdown/learning-objectives directory
- The reflection.md in writing has at least 500 word(s) in total
- The reflection.md in writing has exactly 0 of the `Add Your Name Here` fragment
- The reflection.md in writing has exactly 0 of the `TODO` fragment
- The reflection.md in writing has exactly 1 of the `list` tag
- The reflection.md in writing has exactly 3 of the `code_block` tag
- The reflection.md in writing has exactly 5 of the `code` tag
- The reflection.md in writing has exactly 8 of the `heading` tag
- The repository has at least 5 commit(s)
- The web-development.md in src/markdown/learning-objectives has at least 8 of the `list` tag
- The web-development.md in src/markdown/learning-objectives has exactly 0 of the `TODO` fragment
- The web-development.md in src/markdown/learning-objectives has exactly 1 of the `heading` tag
- The web-development.md in src/markdown/learning-objectives has exactly 1 of the `**Performing Web Development**` fragment
- The web-development.md in src/markdown/learning-objectives has exactly 1 of the `**Using Version Control Systems**` fragment
- The web-development.md in src/markdown/learning-objectives has exactly 1 of the `**Using Web Development Tools**` fragment

```
        ┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
        ┃ Passed 17/17 (100%) of checks for cs302-F2020-lab1! ┃
        ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛
```

## Assignment Assessment

Taking inspiration from the principles of [specification-based
grading](https://www.amazon.com/Specifications-Grading-Restoring-Motivating-Students/dp/1620362422),
the grade that a student receives on a laboratory assignment will be based on
whether or not it meets the standards for technical work in the fields of
software engineering and discrete structures. Instead of receiving a single
numerical or letter grade for this assignment, your grade will have the
following components:

- **Percentage of Correct GatorGrader Checks Ranging Between 0 and 100**: Your
  submitted Python program must pass all of GatorGrader's checks by, for
  instance, ensuring that it produces the correct output and has all of the
  required characteristics. Your technical writing must pass all of
  GatorGrader's checks about, for instance, the length of its output and its use
  of the required Markdown language features for technical writing. For this
  component of a laboratory assignment's grade, your work will receive a
  percentage, ranging from 0 to 100, that corresponds to the percentage of
  GatorGrader checks that automatically pass inside of a GitHub Actions build.

- **GitHub Actions Build Status of Either ✔  or ❌**: Since additional checks on
  the Python source code and/or technical writing are encoded in GitHub Action
  workflows and, moreover, all of the GatorGrader checks are also run in GitHub
  Actions, your work will receive a checkmark grade if the last
  before-the-deadline build in GitHub Actions passes and a ✔  appears in the
  GitHub commit log instead of an ❌. The build status reported by GitHub
  Actions will only be a ✔ if the source code and technical writing in the
  GitHub repository pass all of both the GatorGrader checks and the additional
  checks.

- **Technical Writing Mastery of Either ✔  or ❌**: Students will also receive a
  ✔ grade when the responses to the technical writing questions presented in the
  `writing/reflection.md` reveal a mastery of technical writing skills. To
  receive a checkmark grade, the submitted writing should have correct spelling,
  grammar, punctuation, and formatting in addition to following the rules of the
  Markdown language. Your work will receive a ✔ grade for this component
  if the build report from GitHub Actions reveals that there are no detected
  mistakes in the technical writing.

- **Technical Knowledge and Skill Mastery of Either ✔  or ❌**: Students will
  also receive a checkmark grade when the GitHub repository reveals that they
  have mastered all of the technical knowledge and skills developed during the
  completion of the laboratory assignment. As a part of this grade, the
  instructor will assess aspects of the project including, but not limited to,
  the use of effective Python source code comments, correct Git commit messages,
  and accurate responses to the technical writing questions.

## Advance Feedback on an Assignment

Students who wish to receive feedback on their work for any course assignment
should first open an issue on the issue tracker for their assignment's GitHub
repository, giving an appropriate title and description for the type of feedback
that you would like the course instructor to provide. After creating this issue,
you will see that GitHub has created a unique web site that references it. To
alert the course instructor to the fact that the issue was created and that you
want feedback on your work, please send it to him by a Slack direct message at
least 24 hours in advance of the project's due date. After the instructor
responds to the issue, please resolve all of the stated concerns and participate
in the discussion until the issue is resolved and ultimately marked as closed.

## Discussion of a Graded Assignment

Students who wish to receive feedback on their work for any graded course
assignment should leave question in the same region of Github where the course
instructor submitted the assignment's grade. For example, if the instructor
submits your grade to a pull request in your repository for a laboratory
assignment, then you should ask questions about your grade in that pull request,
bearing in mind the need to @-mention the course instructor in the body of your
comment. Students can continue to discuss the graded assignment with the course
instructor until they understand all the technical topics that were the
focus of the particular assignment.

## Additional Resources

### System Commands

This project invites students to enter system commands into a terminal window.
This assignment uses [Docker](https://www.docker.com) to deliver programs, such
as `gradle` and the source code and packages needed to run
[GatorGrader](https://github.com/GatorEducator/gatorgrader), to a students'
computer, thereby eliminating the need for a programmer to install them on their
development workstation. Individuals who do not want to install Docker can
optionally install of the programs mentioned in the [Project
Requirements](#requirements) section of this document.

### Using Docker

Once you have installed [Docker
Desktop](https://www.docker.com/products/docker-desktop), with MacOS and Linux
you can use the following `docker run` command to start `gradle grade` as a
containerized application, using the
[DockaGator](https://github.com/GatorEducator/dockagator) Docker image available
on
[DockerHub](https://cloud.docker.com/u/gatoreducator/repository/docker/gatoreducator/dockagator).

```bash
docker run --rm --name dockagator \
  -v "$(pwd)":/project \
  -v "$HOME/.dockagator":/root/.local/share \
  gatoreducator/dockagator
```

The aforementioned command will use `"$(pwd)"` (i.e., the current working
directory) as the project directory and `"$HOME/.dockagator"` as the cached
GatorGrader directory. Please note that both of these directories must exist,
although only the project directory must contain something. Generally, the
project directory should contain the source code and technical writing for this
assignment, as provided to a student by the instructor through GitHub.
Additionally, the cache directory should not contain anything other than
directories and programs created by DockaGator, thus ensuring that they are not
otherwise overwritten during the completion of the assignment. To ensure that
the previous command will work correctly, you should create the cache directory
by running the command `mkdir $HOME/.dockagator` on the MacOS and Linux
operating systems. However, if you are using the Windows operating system then
you will instead need to type the command `mkdir
%HomeDrive%%HomePath%/.dockagator`. Finally, if the above `docker run` command
does not work correctly on the Windows operating system, you may need to instead
run the following command to adapt to the differences in the `cmd` terminal
window:

```bash
docker run --rm --name dockagator \
  -v "%cd%:/project" \
  -v "%HomeDrive%%HomePath%/.dockagator:/root/.local/share" \
  gatoreducator/dockagator
```

Here are some additional commands that you may need to run when using Docker:

* `docker info`: display information about how Docker runs on your workstation
* `docker images`: show the Docker images installed on your workstation
* `docker container list`: list the active images running on your workstation
* `docker system prune`: remove many types of "dangling" components from your workstation
* `docker image prune`: remove all "dangling" docker images from your workstation
* `docker container prune`: remove all stopped docker containers from your workstation
* `docker rmi $(docker images -q) --force`: remove all docker images from your workstation

### Using the Docker Shell

Since the above `docker run` command uses a Docker images that, by default, runs
`gradle grade` and then exits the Docker container, you may want to instead run
the following command so that you enter an "interactive terminal" that will
allow you to repeatedly run commands within the Docker container. Don't forget
that, if you are using the Windows operating system, then you will need to use a
different command to run Docker, as explained previously in this document.

```bash
docker run -it --rm --name dockagator \
  -v "$(pwd)":/project \
  -v "$HOME/.dockagator":/root/.local/share \
  gatoreducator/dockagator /bin/bash
```

Once you have typed this command, you can use the [GatorGrader
tool](https://github.com/GatorEducator/gatorgrader) in the Docker container by
typing the command `gradle grade` in your terminal. Running this command will
produce a lot of output that you should carefully inspect. If GatorGrader's
output shows that there are no mistakes in the assignment, then your source code
and writing are passing all of the automated baseline checks. However, if the
output indicates that there are mistakes, then you will need to understand what
they are and then try to fix them.

To run one of these commands, you must be in the main (i.e., "home base")
directory for this assignment where the `build.gradle` file is located. Finally,
please note that students who are using Windows 10 Pro may need to run the
Windows versions of these commands on a long single line in the terminal window.

### Downloading Project Updates

If the course instructor pushes updates to this assignment and you received it
through GitHub Classroom and you would like to also receive these updates, then
you can type this command in the main directory for this assignment:

```
git remote add download git@github.com:Allegheny-Computer-Science-302-F2020/cs302-F2020-lab1-starter/
```

You should only need to type this command once; running the command additional
times may yield an error message but will not negatively influence the state of
your Git repository. Now, you are ready to download the updates provided by the
GatorGrader maintainers by typing this command:

```
git pull download master
```

This second command can be run whenever the course instructor needs to provide
you with new source code for this assignment. However, please note that, if you
have edited the files that we updated, running the previous command may lead to
Git merge conflicts. If this happens, you may need to manually resolve them with
the help of the instructor or a student technical leader. Finally, please note
that the [Gradle plugin](https://github.com/GatorEducator/gatorgradle) for
[GatorGrader](https://github.com/GatorEducator/gatorgrader) will automatically
download the newest version of GatorGrader.

### Using GitHub Actions

This assignment uses [GitHub Actions](https://github.com/features/actions) to
automatically run [GatorGrader](https://github.com/GatorEducator/gatorgrader)
and additional checking programs every time you commit to your GitHub
repository. The checking will start as soon as you have accepted the assignment
&mdash; thus creating your own private repository &mdash; and the course
instructor and/or GitHub enables GitHub Actions on it. If you do not see either
a yellow &#9679; or a green ✔ or a red ❌ in your listing of commits, then
please ask the course instructor to see whether or not GitHub Actions was
correctly enabled.

### System Requirements

This assignment was developed to work with the following software and versions:

- Docker Desktop
- Operating Systems
  - Linux
  - MacOS
  - Windows 10 Pro
  - Windows 10 Enterprise
- Programming Language Tools
  - Gradle 6.6
  - MDL 0.5.0
  - Python 3.7 or 3.8

### Reporting Problems

If you have found a problem with this assignment's provided source code or
documentation, then you can go to the [Computer Science 302 Fall 2020 Planning
Repository](https://github.com/Allegheny-Computer-Science-302-F2020/cs302-F2020-plans)
and [raise an
issue](https://github.com/Allegheny-Computer-Science-302-F2020/cs302-F2020-plans/issues).
If you have found a problem with the [GatorGrader
tool](https://github.com/GatorEducator/gatorgrader) and the way that it checks
your assignment, then you can also [raise an
issue](https://github.com/GatorEducator/gatorgrader/issues) in that repository.
To ensure that your issue is properly resolved, please provide as many details
as is possible about the problem that you experienced. Individuals who find, and
use the appropriate GitHub issue tracker to correctly document, a mistake in any
aspect of this assignment will receive extra credit towards their grade for the
course.

### Receiving Assistance

If you are having trouble completing any part of this project, then please talk
with either the course instructor or a student technical leader during the
course session. Alternatively, you may ask questions in the Slack workspace for
this course. Finally, you can schedule a meeting during the course instructor's
office hours.
