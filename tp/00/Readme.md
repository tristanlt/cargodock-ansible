<!--
---
title: CargoDock - Découvert de Ansible
separator: <!--s-->
verticalSeparator: <!--v-->
theme: blood
css:
    - custom.css
    - assets/css/fontawesome.all.css
revealOptions:
    transition: 'fade'
---
-->
# TP 00 Mode Adhoc

Le but de cette partie est de se familiariser avec les concepts de Ansible en lançant les opérations à la main.

Modules :
- ping
- file
- setup

<!--s-->

### Module Ping

Le module ping ne ferra pas un ping ICMP, il va se connecter sur la ou les machines cibles et répondre pong si cette opération est un succès.

Commande adhoc pour le ping
```bash
ansible test-server -m ping
```

Parfois, il est necessaire de passer en mode de haute verbosité. C'est très instructif, y compris pour comprendre mécanisme de Ansible.
```
ansible -vvvv test-server -m ping
```
<!--s-->
### Utilisation du module file

Le module **file** permet de gérer les fichiers et dossiers. Il prend donc des paramêtres, contrairement à **ping**.

```bash
ansible test-server -m file -a "path=/home/ubuntu/workdir state=directory"
```
[Documentation module file](https://docs.ansible.com/ansible/latest/modules/file_module.html#file-module)

<!--s-->

### Utilisation du module setup

Le module setup est très pratique, mais nous nous en servons jamais de manière explicite. C'est une module interne de Ansible. Il permet de construire le dictionnaire des faits et affiche ceux-ci lors qu'il est appelé de manière explicite.

```bash
ansible test-server -m setup
```
<!--s-->

### Utilisation du module shell

Le module **uptime** permet de passer des commandes.

```bash
ansible test-server -m shell -a "uptime"
```
<!--s-->
### Ressources 

* [Doc ansible Adhoc](https://docs.ansible.com/ansible/latest/user_guide/intro_adhoc.html)
* [Run your first Ansible commands](https://docs.ansible.com/ansible/latest/user_guide/intro_getting_started.html#copying-and-executing-modules)

<!--s-->