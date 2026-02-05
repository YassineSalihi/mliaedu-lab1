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

~~~sh 
ip a 
~~~

![ip a's output](https://github.com/user-attachments/assets/736d6a79-5ce2-47c7-a815-abc8679bb14c) 

# Vérification de DNS et de PING : 
 ![ip route and ping's output](https://github.com/user-attachments/assets/f3cc19e5-78a1-485c-bb45-9cd88c562643) 

# SNAPSHOT : 
 ![SNAPSHOT](https://github.com/user-attachments/assets/03c70a0b-f20c-41da-9539-6aa00375a0b2) 


# Prépare la cible Android :
 ![adb's output](https://github.com/user-attachments/assets/5dd15f2e-a8c3-4a1b-83aa-d58be756befc) 
