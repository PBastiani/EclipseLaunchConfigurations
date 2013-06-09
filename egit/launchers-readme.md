Git Eclipse Launchers
=====================

[Egit](http://www.eclipse.org/egit) brings a subset of [git version control](http://git-scm.com) commands to Eclipse.
The purpose of these launchers is adding valuable git commands that are not yet supported by Egit.

See also: [EGit/Mapping Git Commands](http://wiki.eclipse.org/EGit/Mapping_Git_Commands)

## Prerequisite ##
- To use these launchers, a native Git installation is required.

- The installation of Egit is also required : the launchers use some of Egit variables.

- A String Substitution for **git_exe** is to define. This definition should reference the git executable:

1. Open the **Run/Debug > String Substitution...** preference page.
* Click on **New...** button.
* Enter 'git_exe' as name.
* Click on **Browse...** button; then, select a git executable.
* Click **OK** to close the dialog box and save your changes.

After installation, the launchers should appear in the **Eclipse ToolBar**.

## Launch configurations ##

| Name        | git command        | Description                             |
|:------------|:-------------------|:----------------------------------------|
| git help    | help <>            | Display help information about git      |
| git diagnose| fsck --strict      | Check the repository                    |
| git list ignored files | ls-files -oi --exclude-standard | Display ignored files |
| git list ignored directories | ls-files -oi --directory --exclude-standard  | Display ignored directories |
| git status  | status -sb         | Show the working tree status (short-format) |

<> interactive launcher.

The result of these command appear in the Console with a possible use of ANSI Escape sequences. 
Thanks to [ANSI](http://www.mihai-nita.net/eclipse/) plugin, their appear correctly in the console.

Restriction : the progress messages are not displayed in the console :(