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

```bash
# change the install variables as you see fit!
ansible-pull -KU https://github.com/alexhendel/ansible-workstation-config.git -e install_dotnetsdk=no -e install_zsh=no
```

Alternatively clone the repo and execute locally (installation options for ZSH and Dotnet SDK will be asked via interactive prompt):

```bash
git clone https://github.com/alexhendel/ansible-workstation-config.git ws-setup && cd ws-setup && ansible-playbook -K local.yml
```

## Supported Distros

- Debian
- Ubuntu
- PopOS!
- Fedora
