<div align="center">
  <img src="https://github.com/SciBourne/emacs.d/raw/master/img/logo.png" width="250" title="hover text">
  <h1>GNU Emacs packages and configuration</h1>
  <p>This is my simply Emacs configuration files for work on GNU Linux and MS Windows.</p>
</div>

<br>

## Edit configuration

Edit the configuration files as you like. First of all, pay attention to the settings of the UI.

###### Configuration files:

| Path | Description |
| --- | --- |
| ~/emacs.d/init.el | Main initialization file |
| ~/.emacs.d/config | User init files directory |
| ~/.emacs.d/config/packages.el | User packages set for automatically install them at startup |
| ~/.emacs.d/config/extensions.el | Extension, setting and modes |
| ~/.emacs.d/config/theme-gui.el | Color themes and packages setting for GUI |
| ~/.emacs.d/config/theme-tty.el | Color themes and packages setting for TTY |
| ~/.emacs.d/config/keybinding.el | User keybinding |
| ~/.emacs.d/config/locale.el | Encoding setting |
| ~/.emacs.d/config/irc.el | Template setting for RCIRC client |

<br>

## Quick start for GNU Linux

![Screenshot](img/linux.png)

<br>

### Install the `Git` and `Emacs` packages if not already installed

Gentoo-based:
```
sudo emerge -av dev-vcs/git

sudo touch /etc/portage/package.use/app-editors
sudo echo "app-editors/emacs gpm ssl threads xpm zlib X gtk2 imagemagick jpeg png svg" > /etc/portage/package.use/app-editors

sudo emerge -av app-editors/emacs
````

Debian-based:
```
sudo apt install git
sudo apt install emacs
```

RPM-based:
```
sudo yum install git

sudo yum install epel-release
sudo yum install emacs
```

<br>

### Clone this repository to your home directory

```
cd ~/
git clone https://github.com/SciBourne/.emacs.d.git
```

<br>

### Running Emacs as a server

Possibly, this is distro-specific. I give an example for Gentoo Linux.
```
sudo emerge -av app-emacs/emacs-daemon

```














