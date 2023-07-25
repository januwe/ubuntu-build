# ubuntu-build
Ansible playbook to build my ubuntu

## ToDo
----
- [x] oh-my-zsh + theme
- [x] default terminal
- [x] SpaceVim
- [x] Obsidian
- [ ] auditd + laurel / ufw
- [ ] firefox extensions

optional:

- [ ] PrusaSlicer
- [ ] Minecraft

## Steps on fresh install
----
1. Update and install ansible
```sh
sudo apt update && sudo apt install ansible -y
```

2. Install ansible-galaxy requirements
```sh
cd ubuntu-build/ && ansible-galaxy install -r requirements.yml
```

3. Run ansible-playbook
```sh
ansible-playbook main.yml
```

