# dotfiles
Configuration files for i3wm with zsh. At the time of this upload, resulting system looks like this (colors are not accurate):

![Current](https://github.com/canmetan/dotfiles/blob/master/gifs/sc.gif?raw=true)

### Lock screen:

![Lock](https://github.com/canmetan/dotfiles/blob/master/gifs/lock.gif?raw=true)

Touristic Attractions:

- Switches the desktop background every 5 minutes under a given folder.
- Keyboard shortcuts for launching applications, segregated into workspaces according to their functionality.
- Smooth window transitions and opacity settings.
- No window decorations or title bars. Titles are displayed on the top bar with a yellow text.
- Custom lock screen
- CPU usage, RAM usage, CPU temperature, wifi signal strength, volume, screen brightness, battery level, date and time displayed on the top bar.

Required software (might be misisng a few):

- i3wm (you can possibly incorporate i3-gaps, never tried)
- py3status for the top bar.
- FontAwesome for the fonts used in title bars and for the powerline theme for urxvt terminal.
- compton (for smooth window transitions and transparency)
- xbacklight for adjusting screen backlight on the fly
- PulseAudio for volume control
- lm-sensors (for displaying CPU temp)
- feh (for changing the background image)

How to get a consistent dark theme on Debian (likely to be the same for others):

- Install lxappearance for changing the theme
- Install Xfce-dusk-gtk3 theme (which also includes a gtk 2 theme) under ~/.themes folder or any other theme that has both gtk2 and gtk3+ themes.
- Programs like Thunderbird, Firefox, Spyder and VLC use Qt as their back end which GTK themes do not apply. So if you want to get a dark theme for those applications, follow the instructions listed in [this video](https://www.youtube.com/watch?v=rP4DWu24ff0):
    - Open ~/.config/Trolltech.conf and add style=GTK+ under [Qt] section. If it doesn't exist simply add a [Qt] section.
    - For Debian/Linux Mint/Ubuntu: sudo apt-get install qt5-style-plugins 
    - For Arch Linux: sudo pacman -S qt5-styleplugins 
    - In the file /etc/environment add lines: QT_QPA_PLATFORMTHEME=gtk2 and restart.
    - If you still have a white background (I did), add QT_STYLE_OVERRIDE=gtk2

Terminal used in the screencast: 

- rxvt-unicode
- zsh (with oh-my-zsh, powerlevel9k theme)

Desktop configuration used:

1. Main workspace (IDEs)
1. Secondary workspace (Text editors and program outputs)
1. File system
1. Web browsers
1. Document Editing (LaTeX, libre office etc.)
1. Document Reading (For PDFs mostly)
1. Image manipulation (Gimp, Pinta etc.)
1. Social apps
1. Email
1. Multimedia (cmus, vlc etc.)

If you're going to use keyboard shortcuts for launching applications, make sure to modify the lines on the bottom of the ".config" file.

Modified keyboard shortcuts:

- Super + Right Alt = Closes applications
- Super + F         = Full screen
- Super + Shift + X = Screen lock
- Super + Return    = Terminal

And many others (see ".config" file for details). Please let me know if I've missed anything and thanks for visiting.