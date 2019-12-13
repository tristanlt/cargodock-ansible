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


## CargoDock Ansible

<i class="fas fa-user-astronaut"></i>  Tristan Le Toullec
<i class="fab fa-twitter"></i> tristanlt 

<i class="fa fa-calendar-alt" style="margin-left: 50px"></i> 2 février 2020
<i class="fa fa-map-marker-alt"></i> IUEM Amphi D

![ansible-logo](assets/ansible-logo-bleu.png) <!-- .element height="20%" width="20%" -->
![cargo-logo](assets/logo-cargo-carre-pourfondnoir-200px.png) <!-- .element height="20%" width="20%" -->

<!--s-->

# Ansible 101

<!--s-->

## Que dit Ansible sur Ansible ?

> Ansible is a universal language, unraveling the mystery of how work gets done. Turn tough tasks into repeatable playbooks. Roll out enterprise-wide protocols with the push of a button.

<!--s-->

### Mission ?

 * Gestion des configurations
 * Déploiement d'infrastucture
 * Automatisation
 * Administration en parallèle

<!--s-->

### Spécificité

 ***Sans-agent***

Traduit les actions en Python pour s'executer sur la cible (via SSH). <!-- .element: class="fragment" -->
 
 ***Sans-master***
 
Pas besoin de serveur<!-- .element: class="fragment" -->
 
***Recettes en YAML***

<p><i class="fa fa-heart" style="margin-left: 50px"></i> et <i class="fa fa-bomb" style="margin-left: 50px"></i><i class="fa fa-bomb" style="margin-left: 50px"></i><i class="fa fa-bomb" style="margin-left: 50px"></i></p><!-- .element: class="fragment" -->

***Écrit en Python***

<p><i class="fa fa-heart" style="margin-left: 50px"></i></p><!-- .element: class="fragment" -->

<!--s-->

[On passe à la suite ?](10-start.md)
