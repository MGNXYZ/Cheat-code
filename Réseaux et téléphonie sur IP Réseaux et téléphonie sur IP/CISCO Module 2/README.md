<p align="center">
<a href="[https://user-images.githubusercontent.com/95431446/169254026-e9b9e9d2-7027-4733-ae36-9c0ff3dd31d5.png](https://static.zerochan.net/Yor.Briar.full.3635982.gif)">
<img src="https://static.zerochan.net/Yor.Briar.full.3635982.gif"/>
</a>
</p>


# Navigation IOS

## TP 2

![image](https://user-images.githubusercontent.com/95431446/170012470-e857cf91-b618-4bad-a253-af9dce61e217.png)

![image](https://user-images.githubusercontent.com/95431446/170018551-e59295ac-2ab1-4ea8-87d0-dae5a7db1073.png)
_Terminal_

Étape 2 : Établissez une session de terminal avec S1.

Quelle est la valeur du paramètre des bits par seconde ?
>9600

Quelle est l'invite affichée à l'écran ?
>C2960 Boot Loader

Étape 3 :   Découvrez l'aide IOS.

Quelle commande commence par la lettre « C » ?
>connect

À l'invite, saisissez t, suivi d'un point d'interrogation (?).
Quelles sont les commandes affichées ?
>telnet  terminal  traceroute 

À l'invite, saisissez te, suivi d'un point d'interrogation (?).
Quelles sont les commandes affichées ?
>telnet  terminal

Étape 4 :   Passez en mode d'exécution privilégié.

Quelle information affichée décrit la commande enable ?
>Turn on privileged commands

Que se passerait-il si vous saisissiez <Tab> à l'invite ?
>Tabulation permet de compléter une commande
  
Entrez la commande enable, puis appuyez sur Entrée. Quel changement observez-vous sur l'invite ?
>On passe en mode privilege
  
Étape 5 :   Passez en mode de configuration globale.

Quel est le message affiché ?
>Configuring from terminal, memory, or network [terminal]?

Quel changement observez-vous sur l'invite ?
>On passe en mode config
  
## TP 3
  
a. Saisissez show arp à l'invite.

Notez les adresses MAC et IP indiquées.
>0060.70B4.A601
>
>![image](https://user-images.githubusercontent.com/95431446/170032608-921640f3-e9f4-458e-a510-df47d2bf3d87.png)

Saisissez show flash à l'invite.

Notez l'image IOS indiquée :
>![image](https://user-images.githubusercontent.com/95431446/170032508-2aa8acc5-74f1-445c-8e37-04158f83b576.png)
  
Saisissez show ip route à l'invite.

Combien de routes figurent dans la table ?
>2
>
>![image](https://user-images.githubusercontent.com/95431446/170032827-f38a8a25-e2cf-487c-ae86-65b55fb1e16c.png)
  
Saisissez show interfaces à l'invite.

Quelle interface fonctionne correctement ?
  
>GigabitEthernet 0/0
>
>![image](https://user-images.githubusercontent.com/95431446/170033338-e22527ba-0790-49a9-95ef-04f80c2cf024.png)

b. Saisissez show version à l'invite.

Quelles sont les versions des composants technologiques activés sur le routeur ?

>Version 15.1(4)M4
>
>![image](https://user-images.githubusercontent.com/95431446/170036209-474459d8-9c71-4cd8-acf5-875a18912c17.png)

Saisissez show ? à l'invite. Citez quelques commandes show supplémentaires parmi celles qui sont disponibles en mode d'exécution utilisateur.

>![image](https://user-images.githubusercontent.com/95431446/170036438-e5cdabb6-b5fa-47f3-a9f7-71f1497da85c.png)

c. Saisissez enable à l'invite pour passer en mode d'exécution privilégié. Citez quelques commandes show supplémentaires disponibles dans ce mode.

>![image](https://user-images.githubusercontent.com/95431446/170036510-05bf7107-2ba1-4cfc-960a-3e5bffe6e0b7.png)
  
## TP4
  
![image](https://user-images.githubusercontent.com/95431446/170036775-9efb9b19-6c52-4b49-9f91-1fe84c2f7850.png)

Partie 1 : Effectuer la configuration de base des commutateurs S1 et S2
  
>![image](https://user-images.githubusercontent.com/95431446/170037098-359175b0-ebb1-4792-a5b7-110206fe20f1.png)

Étape 2 : Configurez le mot de passe de console ainsi que celui du mode d'exécution privilégié.
  
>![image](https://user-images.githubusercontent.com/95431446/170037857-6621aa4c-ef98-4818-91b8-e58052f3238b.png)

Étape 3 : Vérifiez les configurations des mots de passe pour S1.

a.Pour vérifier la bonne configuration des mots de passe, saisissez end afin de quitter le mode de configuration globale.
Saisissez exit pour quitter le mode d'exécution privilégié.

>![image](https://user-images.githubusercontent.com/95431446/170038512-1878278c-7907-4f4d-8e52-8d640040cddd.png)

b.Appuyez sur Entrée et vous serez invité à saisir un mot de passe pour accéder au mode d'exécution utilisateur.
  
Quel mot de passe avez-vous utilisé ?
  
>Cisco
  
c.Saisissez enable pour passer en mode d'exécution privilégié. Saisissez le mot de passe lorsque vous y êtes invité.

Quel mot de passe avez-vous utilisé ?
  
>class

d.Saisissez configure terminal pour passer en mode de configuration globale. 

Étape 4 : Configurer une bannière MOTD (message of the day, ou message du jour).
  
>![image](https://user-images.githubusercontent.com/95431446/170040985-b53a37e0-e592-4306-a49f-f95006eca228.png)

  
Étape 5 : enregistrez le fichier de configuration dans la mémoire NVRAM.
  
>![image](https://user-images.githubusercontent.com/95431446/170041262-73370a56-1b9d-46b7-8614-d19c635f283d.png)

Étape 6 : Répétez les étapes 1 à 5 pour S2.
  
### Partie 2 : Configurer les ordinateurs
  

Étape 1 : Configurez les deux ordinateurs en leur attribuant des adresses IP.

>![image](https://user-images.githubusercontent.com/95431446/170042448-1cdc553a-78ec-4348-8202-a97112332f01.png)

>![image](https://user-images.githubusercontent.com/95431446/170042608-4ea0d8ea-1358-4896-9f77-012b7e50acc5.png)

Étape 2 : Testez la connectivité avec les commutateurs.
  
b.Saisissez la commande ping et l'adresse IP de S1, puis appuyez sur Entrée.
 
Avez-vous réussi ? Expliquez votre réponse.  

>Non car S1 n'a pas encore d'adresse ip configurer
  
### Partie 3 : Configurer l'interface de gestion des commutateurs
  
a.En mode de configuration globale, saisissez les commandes suivantes pour configurer S1 avec une adresse IP dans le réseau local virtuel VLAN 1.
  
>![image](https://user-images.githubusercontent.com/95431446/170043784-2501e51e-d88f-4452-b181-2b5d2b145601.png)

À quoi sert la commande no shutdown ?

>Activez l'interface virtuelle
  
b.Enregistrez la configuration.
 
>![image](https://user-images.githubusercontent.com/95431446/170044644-88a7cc96-d48e-4f4c-b99c-4110fbd24b31.png)

c.Vérifiez la configuration de l'adresse IP sur S1 et S2.  
  
>![image](https://user-images.githubusercontent.com/95431446/170045079-4cbafb5a-9715-4f82-bea9-6749c89d2645.png)

  
### Étape 3 : Vérifiez la connectivité du réseau.

>![image](https://user-images.githubusercontent.com/95431446/170045899-0ad3b5ed-e93f-455d-8fe5-5811f3076e29.png)
> 
>![image](https://user-images.githubusercontent.com/95431446/170046052-f833e815-01ec-48b4-8ee3-37d5a76c4933.png)
>
>![image](https://user-images.githubusercontent.com/95431446/170046235-5166597d-a180-49c8-af5d-e219b140ed4b.png)


  
>![image](https://user-images.githubusercontent.com/95431446/170047381-f934bc5e-faf8-42ef-9441-52eddd93d5ff.png)

  
  
  


  
  
