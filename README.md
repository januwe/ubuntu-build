# ubuntu-build
Ansible playbook to build my ubuntu

## ToDo
----
- [x] oh-my-zsh + theme
- [x] default terminal
- [x] SpaceVim
- [ ] auditd + laurel / ufw
- [X] mount `/tmp` on tmpfs
- [X] disable system crash reports
- [X] install oh my zsh
- [X] set default editor to vim instead of nano 
- [X] enable fstrim for better ssd lifetime 
- [ ] install flatpak and add flathub remote
- [ ] install podman + distrobox 
- [ ] configure distrobox
- [ ] configure bat, exa, zoxide, navi for zsh

## Steps on fresh install
----
1. Update and install ansible
```sh
sudo apt update && sudo apt install ansible git -y
```

2. Install ansible-galaxy requirements
```sh
git clone git@github.com:januwe/ubuntu-build.git
cd ubuntu-build/
ansible-galaxy collection install community.general
```

3. Run ansible-playbook
```sh
ansible-playbook -i inventory main.yml -e local_user=<user> -K
```

