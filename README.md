# Workstation Tools

This repository contains scripts to automate and speedup the workflow and preparation for my machine.

> **_Disclaimer_** :  
> Those scripts are ubuntu related with major version 18+, for other distributions you'll need to adapt it
___

## Prepare Workstation

> Leia o arquivo `ubuntu.yml` antes de rodar os comandos abaixo e habilite/desabilite os blocos que lhe interessarem.

1. Instalação Ansible
```bash
sudo apt update && sudo apt install ansible unzip git -y
```
2. Clonar o repositório
```bash
git clone https://github.com/prhirata/developer-tools.git
```

3. Aplicar a configuração especificada no `ubuntu.yml`
```bash
ansible-playbook tools/ubuntu.yml --ask-become-pass
```
>Digite sua senha quando solicitado para dar permissão root em algumas ações.
___

## Testing playbook on Multipass VM

Access url: https://www.ivankrizsan.se/2021/05/16/ansible-and-multipass-virtual-machines/

# License
GPLv3

# Author Information
Created by [Caio Delgado](https://linktr.ee/caiodelgadonew)

Contributions are more than welcome!

Modified by [Paulo Hirata]