# TP 00 Mode Adhoc

Lancer des opérations en utilisant des modules Ansible.

Modules :
- ping
- file

### Ping le test SSH 

Le module ping n'est pas un ping ICMP, il va se connecter sur la ou les machines cibles et répondre pong si cette opération est un succès.

Commande adhoc pour le ping
```bash
ansible test-server -m ping
```
Ça marche ? Passons en debug...
```
ansible -vvvv test-server -m ping
```

### Utilisation du module file

Le module **file** permet de gérer les fichiers et dossiers. Il prend donc des paramêtres, contrairement à **ping**.

```bash
ansible test-server -m file -a "path=/home/ubuntu/workdir state=directory"
```

### Utilisation du module shell

Le module **uptime** permet de passer des commandes.

```bash
ansible test-server -m shell -a "uptime"
```



### Ressources 

* [Doc ansible Adhoc](https://docs.ansible.com/ansible/latest/user_guide/intro_adhoc.html)
* [Run your first Ansible commands](https://docs.ansible.com/ansible/latest/user_guide/intro_getting_started.html#copying-and-executing-modules)

