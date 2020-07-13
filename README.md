How to Install MultiMC on Arch Linux ARM/Manjaro ARM

1. git clone https://aur.archlinux.org/multimc-git.git
2. cd multimc-git
 3. Modify PKGBUILD by replacing `arch=('i686' 'x86_64'`) with `arch=('aarch64')`
 4. makepkg -si

MultiMC should now compile and will be installable

You can install my compiled version by doing `sudo pacman -U multimc-git-0.6.11.r31.gcd57e354-1-aarch64.pkg.tar.xz`
My compiled version was built on my Pi 4 running Manjaro ARM

Note use this [patcher](https://github.com/JJTech0130/MultiMC-Patcher) to make Minecraft to run
