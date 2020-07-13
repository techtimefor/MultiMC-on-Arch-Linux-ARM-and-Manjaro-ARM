How to Install MultiMC on Arch Linux ARM/Manjaro ARM

1. git clone https://aur.archlinux.org/multimc-git.git
2. cd multimc-git
 3. Modify PKGBUILD by replacing `arch=('i686' 'x86_64'`) with `arch=('aarch64')`
 4. makepkg -si

MultiMC should now compile and will be installable
