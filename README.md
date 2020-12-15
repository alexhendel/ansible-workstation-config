# Local Linux Workstation Setup

This Ansible script sets up a ZSH working environment with:

- [zsh](https://github.com/zsh-users/zsh)
- [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh)
- [powerlevel10k zsh theme](https://github.com/romkatv/powerlevel10k) and
- [nvm](https://github.com/nvm-sh/nvm)

It also does:

- update & upgrade all packages to latest version
- add some git configuration

## Run the Script

To run the setup script `sudo apt install -y ansible git` must be run first.

Then go ahead and run:

```
ansible-pull -KU https://github.com/alexhendel/ansible-workstation-config.git
```

## Supported Distros

- Debian
- Ubuntu
- PopOS!
