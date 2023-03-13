# MacOS

https://www.youtube.com/watch?v=CF1tMjvHDRA

# Ubuntu

Source : https://www.youtube.com/watch?v=-s3Yjzu4P4o

### Prepare system and install zsh
`sudo apt update`

`sudo apt install zsh`

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

If prompted "Change default shell to zsh, choose yes or not".
Je pense qu'il est mieux de garder "NO".

Check version and location of SHELL
`$SHELL --version`

`echo $SHELL`

### Powerlevel10k

`git clone --depth=1 git@github.com:romkatv/powerlevel10k.git ~/powerlevel10k`

`echo 'source ~/'powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc`

`exec zsh`

Configurer ensuite powerlevel10k.

Conclure avec :
`sudo apt update`


### Fix Oh My ZSH Inseure

Fix Oh My Zsh “Insecure completion-dependent directories detected”.
ZSH complains about permissions.

https://osxdaily.com/2021/12/29/fix-oh-my-zsh-insecure-completion-dependent-directories-detected/

`chmod 755 /usr/local/share/zsh`

`chmod 755 /usr/local/share/zsh/site-functions`

Default are 775.





