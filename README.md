# ubuntu-build
Ansible playbook to build my ubuntu

## ToDo
----
- [ ] oh-my-zsh + theme
- [ ] default terminal
- [ ] firefox extensions

## Steps on fresh install
----
1. Update and install ansible
```sh
apt update && apt install ansible -y
```

2. Install ansible-galaxy requirements
```sh
ansible-galaxy install -r requirements.yml
```

3. Run ansible-playbook
```sh
ansible-playbook main.yml
```

