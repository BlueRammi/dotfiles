Scripts:
* **adv_windowlist**: Use `awl_viewer = "yes";` to fit the windows list into a tmux pane.
* **autoaway**: TODO: Enable it automatically when Irssi starts.
* **buffer**: Great script to copy and paste text inside Irssi.
* **calc**: Useful script to make arithmetic operations inside Irssi.
* **cleanpublic**: Remove colors in public channels, so we can read black text as white.
* **go2**: This command is mapped to `^G` (ctrl+g) to go to a window.
* **idletime**: It retrieves the idletime of any nickname.
* **openurl**: List the saved URLs.
* **scriptassist**: Really useful script manager. It checks for updates, as well!
* **sysinfo_dg**: This script prints the current system info in a channel.
* **tmux-nicklist-portable**: It's awesome to see a nick list into a tmux pane.
* **trackbar22**: It adds an horizontal line to remember the last line we read.
* **usercount**: Count the users of a channel and display it in the status bar.
* **desktop-notify**: Display desktop notifications when a message is received.

There are two ways to install the scripts:

1. Using **scriptassist** (however, you must have it already installed into `~/.irssi/scripts/`).

	- For example, let's install the script **buffer**:
	`/scriptassist install buffer`

	- Now, let's create the symlink to the `autorun` folder:
	`/scriptassist autorun buffer`

	- We also can check for updates:
	`/scriptassist check`

	- Or even search scripts with a keyword:
	`/scriptassist search buffer`

2. Using the bash script I created. It's useful for the first install in a machine. The script file is called **iip.sh**. Execute it:
`. ./iip.sh`

	Execute it from everywhere, and it will download the scripts listed above into your `~/.irssi/scripts/` directory. It will create the symlinks to the `autorun` subdirectory, as well.

---

Note that **scriptassist** requires to have some perl modules installed.

```
perl-libwww
perl-lwp-protocol-https
perl-text-charwidth
perl-glib-object-introspection
```

It's not required to install them through CPAN if these packages are in the repositories of your distro. In Manjaro (Arch Linux based), they are.
