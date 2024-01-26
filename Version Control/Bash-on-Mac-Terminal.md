# Using Bash on Mac Terminal

## Learning Objectives

- Learners will understand how to open the command line - terminal on Mac.
- Learners will become familiar with the most common commands.

## Mac Terminal

The Terminal on Mac can be opened in one of three ways: Finder, Launch Pad, and Spotlight.

### Finder

1. Scroll to the bottom of your desktop and click on the Finder icon.
2. Click on Applications on the left-hand side of the screen.
3. Locate the folder called Utilities and expand it.
4. The Terminal app should be visible, select it to open.

*Applications list in the Finder window with Terminal highlighted.*

### Launch Pad

1. Press the F4 command.
2. Launch Pad view appears onscreen.
3. Select the search bar and type Term (short for Terminal).
4. The Terminal icon appears onscreen.
5. Select the icon to open.

*Terminal icon in the Launch pad.*

### Spotlight

1. Press the command key and the space bar.
2. The Spotlight modal appears.
3. Type in the word Terminal or Term for short.
4. The Terminal icon appears onscreen.
5. Select the icon to open the Terminal.

*Spotlight modal with the word Terminal entered in the search bar.*

## Bash Commands

Bash provides a list of commands for navigating through files, viewing the contents of files, and edit features for changing or updating the contents of a file. Below is a list of the most common commands:

| Command | Used for |
| --- | --- |
| cd | Change Directory |
| ls | List command used for showing the content of a directory |
| rm | Remove command used for removing a file or a directory |
| mv | Used to move files or folders to another location |
| touch | Allows creating a new empty file or updating a timestamp on a file |
| cp | Used to make a copy of a file or folder |
| mkdir | Make a new directory |
| pwd | Print work directory, shows the current location in the shell |
| cat | Allows reading or concatenation of a file |
| less | Displays the contents of a file one page at a time |
| grep | Global regular expression, allows for searching contents of files or folders |

### Flags

Every bash command has flags for changing the output of the command itself. For example, the `ls` command prints out the list of contents inside a directory. If we wanted to show the list in a different view, we simply need to add a flag such as `-l`.

*Terminal window showing the output from the ls command.*

When the flag of `-l` is passed, it will show the output differently:

*Terminal window showing the output from the ls -l command.*

### Man Pages

When first learning commands from bash, it can feel a bit daunting. Luckily, every command has its manual (or man pages for short). The man page lists all the flags and options that a particular command has to offer. Again, let's use the `ls` command to demonstrate this. Type the following:

```bash
man ls

```

# The General Commands Manual in the Terminal window

The man pages are a great way to recall the different flags that are available and a great tool in your arsenal to becoming more fluent in bash.

## Editing

There are many options for editing files in bash. The most common is usually VI or Vim. VI stands for visual editor. It's used for making edits and changes to a file and saving them. It's similar to what you may have used in applications like Word. VIM is a better version of VI with some improvements - hence its name: visual editor improved. Learning the commands in Vim will feel different from GUI applications, but once you practice, it will feel like second nature. Vim uses modes to determine the commands you can work with:

- **Normal mode:** Default mode
- **Insert mode:** Allows the contents of the files to be edited.
- **Command line mode:** Normal commands begin with `:`
