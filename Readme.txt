First is create a user in GitHub and send me your username so that I can add you as Collaborators.

Sencond install msysGit from URL http://msysgit.github.com/
After it’s installed, you have both a command-line version (including an SSH client that will come in handy later) and the standard GUI.

First-Time Git Setup

Your Identity

The first thing you should do when you install Git is to set your user name and e-mail address. This is important because every Git commit uses this information, and it’s immutably baked into the commits you pass around:

$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com

Again, you need to do this only once if you pass the --global option, because then Git will always use that information for anything you do on that system. If you want to override this with a different name or e-mail address for specific projects, you can run the command without the --global option when you’re in that project.

Checking Your Settings

If you want to check your settings, you can use the git config --list command to list all the settings Git can find at that point:

$ git config --list
user.name=Scott Chacon
user.email=schacon@gmail.com
color.status=auto
color.branch=auto
color.interactive=auto
color.diff=auto
...

Getting Help

If you ever need help while using Git, there are three ways to get the manual page (manpage) help for any of the Git commands:

$ git help <verb>
$ git <verb> --help
$ man git-<verb>

For example, you can get the manpage help for the config command by running

$ git help config


