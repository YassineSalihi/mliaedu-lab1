1. Installing Mobexler.ova
2. check integrity with "sha256sum" command.
3. Attendre l'import.3. Attendre l'import.3. Attendre l'import.

---

# Configuration : 
On crée le nom "vboxnet0" pour qu'on puisse ajouter 
un deuxième Adapter de type "Host-only". 
![create vboxnet0](https://github.com/user-attachments/assets/9b14f553-6625-459d-8399-7757f5854414) 

# Démarrage :  
 On ouvre le terminal, on fait "ip a" 

> [!WARNING]
> On a deux interfaces réseaux, 
> enp0s17 est allumé par défaut.
> enp0s8 doit etre activer par la commande : 
> ~~~sh
> sudo ip link set enp0s8 up 
> ~~~



