MISC Launchers
==============

This folder contains a set of Windows specific launchers.

**Windows Explorer**

Start the Windows Explorer on the selected resource.

**Windows Bash**

Start a Unix-type command-line shell.

As prerequisite, a Bash release for Windows should be installed on the workstation.
Thanks to [msysGit](http://msysgit.github.io/), the developers can use tools like Bash or git from Windows...

As next prerequisite, a String Substitution for **bash_exe** is to define. 
This definition should reference the bash executable:
- Open the **Run/Debug > String Substitution...** preference page.
- Click on **New...** button.
- Enter **bash_exe** as name.
- Click on **Browse...** button; then, select a bash executable.
- Click **OK** to close the dialog box and save your changes.

Note: these launchers use the CMD command. To improve productivity, the use of [Console2](http://sourceforge.net/projects/console/files/) may be considered !