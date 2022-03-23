# Lab 1: Unix Shell

In this lab, we'll be using material from [Software Carpentry](https://swcarpentry.github.io/) related to using the linux/unix command line. We'll work through the material together, but you'll get the most out of the activity if you _actually_ do the work along with me. In a remote environment, it can be hard for me to gauge your interactivity, so you'll get the most out of this if you let me know to slow down, have questions, or are having technical issues.

## The problem we are going to try to solve: Nelle’s Pipeline

Nelle Nemo, a marine biologist, has just returned from a six-month survey of the [North Pacific Gyre](http://en.wikipedia.org/wiki/North_Pacific_Gyre), where she has been sampling gelatinous marine life in the [Great Pacific Garbage Patch](http://en.wikipedia.org/wiki/Great_Pacific_Garbage_Patch). She has 1520 samples that she’s run through an assay machine to measure the relative abundance of 300 proteins. She needs to run these 1520 files through an imaginary program called `goostats.sh` she inherited. On top of this huge task, she has to write up results by the end of the month so her paper can appear in a special issue of _Aquatic Goo Letters_.

The bad news is that if she has to run `goostats.sh` by hand using a GUI, she’ll have to select and open a file 1520 times. If `goostats.sh` takes 30 seconds to run each file, the whole process will take more than 12 hours of Nelle’s attention. With the shell, Nelle can instead assign her computer this mundane task while she focuses her attention on writing her paper.

The next few lessons will explore the ways Nelle can achieve this. More specifically, they explain how she can use a command shell to run the `goostats.sh` program, using loops to automate the repetitive steps of entering file names, so that her computer can work while she writes her paper.

As a bonus, once she has put a processing pipeline together, she will be able to use it again whenever she collects more data.

In order to achieve her task, Nelle needs to know how to:

- navigate to a file/directory
- create a file/directory
- check the length of a file
- chain commands together
- retrieve a set of files
- iterate over files
- run a shell script containing her pipeline

> ### Key Points[](https://swcarpentry.github.io/shell-novice/01-intro/index.html#key-points)
>
> - A shell is a program whose primary purpose is to read commands and run other programs.
> - This lesson uses Bash, the default shell in many implementations of Unix.
> - Programs can be run in Bash by entering commands at the command-line prompt.
> - The shell’s main advantages are its high action-to-keystroke ratio, its support for automating repetitive tasks, and its capacity to access networked machines.
> - The shell’s main disadvantages are its primarily textual nature and how cryptic its commands and operation can be.

## Prior to the lab

1. Download [shell-lesson-data.zip](https://swcarpentry.github.io/shell-novice/data/shell-lesson-data.zip) and move the file to your Desktop. Unzip/extract the file. Let your instructor know if you need help with this step. You should end up with a new folder called shell-lesson-data on your Desktop.
2. We will be using the Terminal window in `Rstudio` for this session. While this is not the usual way to teach these materials, it will allow us to stick to the `Rstudio` environment so that as you work on your R work, you can jump into the shell easily in the future.

IF YOU HAVE Rstudio installed, the following is OPTIONAL, but useful.

1. [Follow the instructions to install the necessary software (just the Shell part)](https://carpentries.github.io/workshop-template/#shell), depending on the operating system that your computer uses.
2. Make sure that you can get to the so-called terminal where you can type commands.
   - On MacOS, make sure that you can run the `Terminal` program. This is in the `Applications` and then `Utilities` folder.
   - On Windows, after installing the software in step 2, go to the Start menu, search for `Git Bash` or choose `All Apps` and then find `Git` and then under that click `Git Bash`. There is a video right below the installation instructions to watch if you need more direction.

## Materials for the Lab

I encourage you to NOT follow along with the lab materials as we work through them. Instead, work with and experiment with me. The lab materials are available here for future reference or to continue after our session ends.

- https://swcarpentry.github.io/shell-novice/
