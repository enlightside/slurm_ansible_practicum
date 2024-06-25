# slurm_ansible_practicum
 
Практикум по Ansible на курсе Slurm

Ansible Host: Ubuntu 22.04 (name: ubuntu)
Target Host: Centos 7 (name: centos7)

Для запуска нужно выполнить шаги

 1. Склонировать репозиторий: 
 `git clone https://github.com/enlightside/slurm_ansible_practicum.git`
 2. Перейти в папку slurm_ansible_practicum
 3. Скопировать ssh-ключ на target host: ssh-copy-id root@centos7
 4. Запустить установку коллекций и ролей с Ansible Galaxy: 
 `ansible-galaxy install -r requirements.yml`
 5. Запустить Ansible Playbook с ключом `--ask-vault-pass`: 
 `ansible-playbook --ask-vault-pass playbook.yml`
