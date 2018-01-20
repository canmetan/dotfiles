# dotfiles
Dot files for i3wm with zsh. At the time of this upload, system looks like this (colors are not accurate):

![Current](https://github.com/canmetan/dotfiles/blob/master/gifs/sc.gif?raw=true)

![Lock](https://github.com/canmetan/dotfiles/blob/master/gifs/lock.gif?raw=true)

Attractions:

- Switches background picture every 5 minutes under a given folder.
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

Please let me know if I've missed anything.
Terminal used in the screenshot 

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