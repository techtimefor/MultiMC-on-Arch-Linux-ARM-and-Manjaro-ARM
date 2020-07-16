How to Install MultiMC on Arch Linux ARM/Manjaro ARM

1. git clone https://aur.archlinux.org/multimc-git.git
2. cd multimc-git
 3. Modify PKGBUILD by replacing `arch=('i686' 'x86_64'`) with `arch=('aarch64')`
 4. makepkg -si
 
 Note if you do not want to modify PKGBUILD you can use the PKGBUILD provided here its updated daily
 Just do `cd $HOME/multimc-git && rm PKGBUILD && wget https://raw.githubusercontent.com/techtimefor/MultiMC-on-Arch-Linux-ARM-and-Manjaro-ARM/master/PKGBUILD`
 Lastly do `makepkg -si`

MultiMC should now compile and will be installable

You can install my compiled version by doing `wget https://github.com/techtimefor/MultiMC-on-Arch-Linux-ARM-and-Manjaro-ARM/blob/master/multimc-git-0.6.11.r31.gcd57e354-1-aarch64.pkg.tar.xz?raw=true && sudo pacman -U multimc-git-0.6.11.r31.gcd57e354-1-aarch64.pkg.tar.xz`
My compiled version was built on my Pi 4 running Manjaro ARM

Note use this [patcher](https://github.com/JJTech0130/MultiMC-Patcher) to make Minecraft to run

The patcher won't work unless you replace `mmcroot="$HOME/MultiMC"` with
`mmcroot="$HOME/.local/share/multimc"`

Credits to [@JJTech0130](https://github.com/JJTech0130) and the Maker of the [Gitlab Snippet](https://gitlab.com/snippets/1933165)
also [MultiMC](https://github.com/MultiMC/MultiMC5)
 
