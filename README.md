# Local Linux Workstation Setup

This Ansible script sets up a ZSH working environment with:

- [zsh](https://github.com/zsh-users/zsh)
- [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh)
- [powerlevel10k zsh theme](https://github.com/romkatv/powerlevel10k) and
- [nvm](https://github.com/nvm-sh/nvm)

To run the setup script `sudo apt install -y ansible git` must be run first.

Then go ahead and run:

```
# remember to change the user id
ansible-playbook --user johnd --ask-become-pass --connection=local --inventory 127.0.0.1, --limit 127.0.0.1 commandline.yml
```
