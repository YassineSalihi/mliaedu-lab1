## Introduction
Ce document décrit les étapes d’installation et de configuration de la machine virtuelle Mobexler, ainsi que les vérifications réseau et la préparation d’une cible Android avant le début des manipulations.

---

1. Installation de Mobexler.ova
2. Vérifier l'intégrité avec la commande "sha256sum".
3. Attendre l'importation.

---

# Configuration : 
On crée le nom "vboxnet0" pour qu'on puisse ajouter 
un deuxième Adapter de type "Host-only". 
![create vboxnet0](https://github.com/user-attachments/assets/9b14f553-6625-459d-8399-7757f5854414) 
*Figure 1 – Création de l’interface réseau Host-only `vboxnet0`*


# Démarrage :  
 On ouvre le terminal, on fait "ip a" 

> [!WARNING]
> On a deux interfaces réseaux, 
> enp0s17 est allumé par défaut.
> enp0s8 doit etre activer par la commande : 
> ~~~sh
> sudo ip link set enp0s8 up 
> ~~~

~~~sh 
ip a 
~~~

![ip a's output](https://github.com/user-attachments/assets/736d6a79-5ce2-47c7-a815-abc8679bb14c) 
*Figure 2 – Affichage des interfaces réseau avec la commande `ip a`*

# Vérification de DNS et de PING : 
On teste la connectivité vers Google pour valider l'accès internet et la résolution DNS.
 ![ip route and ping's output](https://github.com/user-attachments/assets/f3cc19e5-78a1-485c-bb45-9cd88c562643) 
*Figure 3 – Vérification de la connectivité réseau et de la résolution DNS*


# SNAPSHOT : 
On sauvegarde l'état propre de la machine virtuelle avant de commencer les manipulations.
 ![SNAPSHOT](https://github.com/user-attachments/assets/03c70a0b-f20c-41da-9539-6aa00375a0b2) 
*Figure 4 – Création d’un snapshot de la machine virtuelle*

# Prépare la cible Android :
On vérifie que la machine détecte bien le périphérique Android via ADB.
 ![adb's output](https://github.com/user-attachments/assets/5dd15f2e-a8c3-4a1b-83aa-d58be756befc) 
*Figure 5 – Détection du périphérique Android via ADB*

