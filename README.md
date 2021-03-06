# 🍙 FunkyDots
Another portable Arch based system made with love & style. It integrates my desired digital environment.

**uwu**
![showcase img](./.local/share/funkydots/pix/uwu/pic2.png)
![showcase img](./.local/share/funkydots/pix/uwu/pic3.png)
![showcase img](./.local/share/funkydots/pix/uwu/pic4.png)

**cyber**
![showcase img](./.local/share/funkydots/pix/cyber/pic1.png)
![showcase img](./.local/share/funkydots/pix/cyber/pic4.png)

## Some Info
- It also serves as:
  - A learning resource for anyone who wants to customize their environment & learn more about ricing *(e.g conf files, scripts)*
  - A backup for myself in case anything goes wrong
  - An easy & quick way to quickly port my system to another machine
- Check out [my programs](https://github.com/vlagh3/funkydots/blob/main/.local/share/funkydots/progs.md) note to see what's coming with this setup
- To get your way around the system, see [my keybinds](./.local/share/funkydots/keybinds.md) *(feel free to change them as you please)*
- This setup would have not been possible without the help of the greatly genereous open-source community. So I encourage you to take a look at [those projects](#inspiration--kudos) & show some love *(don't be just a taker)*

### Structure
I try to keep things as organized & clean as I possibly can. Thus, I follow the [XDG Base Directory Specification](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html) to structure my `~` directory. Below is a summary:
```bash
~
├── .config		# configs for programs that I use
├── .dtf		# bare repository to manage this repo
├── .local
  ├── share	        # where user data is stored 
    ├── init_install    # helper stuff 4 installing the setup
    ├── startupB	 # custom startup browser page
  ├── bin		# my scripts
  ├── src		# mostly suckless utils (e.g dwm, dwmblocks)
```
- To change the file & directory navigation shortcuts, modify the [dirnav](https://github.com/vlagh3/funkydots/blob/main/.config/shell/dirnav) & [filenav](https://github.com/vlagh3/funkydots/blob/main/.config/shell/filenav) files
  - loaded by the [shortucts](https://github.com/vlagh3/scripties/blob/master/system/shortcuts.sh) script on [zsh](https://www.zsh.org/) startup
- `.profile`, `.zprofile` is linked to the `.config/shell` directory
- `.xprofile`, `.xinitrc` is linked to the `.config/x11` directory
- The loading of environment variables happens in [shell/profile](https://github.com/vlagh3/funkydots/blob/main/.config/shell/profile)

### Submodules

|                                                  |                                                                                   |
| ------------------------------------------------ | --------------------------------------------------------------------------------- |
| [chadwm fork](https://github.com/vlagh3/chadwm)  | dwm as beautiful as possible                                                      |
| [scripties](https://github.com/vlagh3/scripties) | custom bash scripts + other usefull stuff collected *(e.g sec, devops, sysadmin)* |
| [alis fork](https://github.com/vlagh3/alis)      | arch linux install script                                                         |
| [dawn fork](https://github.com/vlagh3/dawn)      | a gracius custom startpage                                                        | 

### Dot-files management
There are multiple ways to manage your dotfiles as seen in numerous articles. I would definitely recommend going through these resources and find the one that suits you the best:
- https://dotfiles.github.io/
- https://hackernoon.com/learn-how-to-manage-dotfiles-b8b62c6c5491
- https://stackoverflow.com/questions/16292409/how-to-use-github-to-manage-dotfiles
- [Ask HN: What do you use to manage dotfiles?](https://news.ycombinator.com/item?id=11070797)

I personally use a [git bare](https://www.keblog.me/2015/01/bare-git-repository/) repository as a result of reading an [awesome article](https://www.atlassian.com/git/tutorials/dotfiles) + it integrates better with my [Submodules](#submodules) & overall workflow. I find it scalable, flexible & pretty easy to use once you get the gist of it. However, it has some downsides as well *(as everything I suppose)*

## Install
To get yourself setup
```bash
# Download arch install scripts (alis)
curl -sL https://raw.githubusercontent.com/vlagh3/alis/master/download.sh | bash
./alis.sh
```

Upon reboot
```bash
# Download my version of larbs & execute it
curl -s https://raw.githubusercontent.com/vlagh3/funkydots/main/.local/share/init_install/larbs.sh -o larbs.sh
sudo bash larbs.sh
```

OR just `git clone https://github.com/vlagh3/funkydots.git` and move everything in your `$HOME`

### Tips & Tricks
- use an url shortener for downloading the scripts *(e.g [git.io](https://git.io/))*
- be sure that the initialization script *([alis.conf](https://github.com/vlagh3/alis/blob/master/alis.conf))* is configured properly for your system
- if you want a minimal install pass the `-p` option to [larbs](https://larbs.xyz/) with the [progs_min.csv file](https://github.com/vlagh3/funkydots/blob/main/.local/share/init_install/progs_min.csv) or your custom one

## Inspiration & Kudos
Grazie
- [OneDark](https://github.com/Mangeshrex/dotfiles)
- [DTOS](https://gitlab.com/dwt1/dtos)
- [larbs](https://github.com/LukeSmithxyz/LARBS)
- [chadwm](https://github.com/siduck/chadwm)
- [alis](https://github.com/picodotdev/alis)
- [NVchad](https://nvchad.github.io/)
- [dawn](https://github.com/b-coimbra/dawn)
- [voidrice](https://github.com/LukeSmithxyz/voidrice)
- [unixporn](https://www.reddit.com/r/unixporn/wiki/index)
- [cozy dots](https://github.com/Macawls/dotfiles)
- [dotfiles 2.0](https://github.com/Axarva/dotfiles-2.0)
- The community

## Contributions & Support

- **Do you have a suggestion or fix?**
  - feel free to open up a [pull request](https://github.com/vlagh3/funkydots/pulls)

- **Having an issue, problem, error?**
  - Don't be shy & open an [issue](https://github.com/vlagh3/funkydots/issues) or ping me
  - "The important thing is not to stop questioning. Curiosity has its own reason for existing."
    - however that doesn't mean you should not read the effin manual



## License
The files and scripts in this repository are licensed under the BS License, which is a permissive license allowing you to use, modify, copy & distribute the software. An important step in accepting to use this licence is to firstly read it & think by your own. If not, you agree to sell your soul to the devil while giving me 1.000.000$. (Also known as the BulShit License)
