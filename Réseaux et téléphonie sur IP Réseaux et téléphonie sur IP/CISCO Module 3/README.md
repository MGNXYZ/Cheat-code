<p align="center">
<a href="[https://user-images.githubusercontent.com/95431446/169254026-e9b9e9d2-7027-4733-ae36-9c0ff3dd31d5.png](https://static.zerochan.net/Yor.Briar.full.3635982.gif)">
<img src="https://static.zerochan.net/Yor.Briar.full.3635982.gif"/>
</a>
</p>


# TP 1 Module 3

## Part 1 : Configuration vlan par défaut

Etape 1 : Voir le vlan de S1

On utilise la commande :

>show vlan brief

>![image](https://user-images.githubusercontent.com/95431446/170227593-ecc6bd31-ce89-4e45-96e0-d4a426105b59.png)

Etape 2 : Vérifier la connectivité entre les pc du même réseau

Quel bénéfice les VLANs apporte au réseau

>Sécurité, efficacité, réduction des couts, meilleurs perfs, gestion simplifiée

## Part 2 : Configuration des VLANs

Etape 1 : Créer et nommée les VLANs sur S1

>![image](https://user-images.githubusercontent.com/95431446/170229494-361ff278-60ba-4f68-89f3-3e04c1d70f9f.png)

Etape 2 : Vérifier la configuration des VLANs

>![image](https://user-images.githubusercontent.com/95431446/170229873-544e2db6-fa59-415c-93d3-3a0a37f67887.png)

Etape 3 : Créer les VLANs sur S2 et S3

>![image](https://user-images.githubusercontent.com/95431446/170231951-12864260-5959-4508-8da3-4b66ffafb751.png)

>![image](https://user-images.githubusercontent.com/95431446/170232006-daef99a6-3dfb-41d3-8290-fd4d791f3922.png)


## Part 3 : Assigné les VLANs a un port 

Etape 1 : Assigné les VLANs de S2 et S3 au port actif

>![image](https://user-images.githubusercontent.com/95431446/170232700-e0639d93-5f96-45db-b500-f6c071f7a186.png)

>![image](https://user-images.githubusercontent.com/95431446/170234622-d4098fcf-ec69-4ef3-a84d-ec45e50a9c8e.png)

>![image](https://user-images.githubusercontent.com/95431446/170235682-b619a739-a643-403f-a271-e0b43f80b800.png)


Etape 2 : Assigné le VLAN VOICE a FastEthernet 0/11 sur S3

>![image](https://user-images.githubusercontent.com/95431446/170236891-631ef86e-8153-4728-89f3-55a03dc6b677.png)

Etape 3 : Test de connectivité

>PC1 ne peux pas ping PC4 car les trunks ne sont pas configuré.


# TP 2 Module 3 : Configure trunks

## Part 1 Verifié les VLANs

Etape 1 : Voir les vlans actuellement en place

>![image](https://user-images.githubusercontent.com/95431446/170253748-64e428fc-6a96-4fc8-ad68-a4fb29c34395.png)

## Part 2 : Configuration des trunks

>![image](https://user-images.githubusercontent.com/95431446/170266047-248273ed-4168-4687-8df5-fd1c07260877.png)
_configuration des trunks sur GigaHeternet 1 et 2_

>![image](https://user-images.githubusercontent.com/95431446/170266663-4557051f-60ea-464c-a590-39767e63219b.png)
_Configuration de VLAN 99 en vlan natif de GO/1 - 2_

Malgré une non-concordance actuelle du VLAN natif, les requêtes ping entre les PC d'un même VLAN aboutissent. Expliquez votre réponse.

Les requêtes ping aboutissent car l’agrégation a été activée sur le commutateur S1. Le protocole DTP a négocié automatiquement l'autre côté des liens trunk. Dans ce cas de figure, les 
commutateurs S2 et S3 ont configuré automatiquement les ports raccordés au commutateur S1 comme des ports de trunking

Étape 2 : Vérifiez que le trunking est activé sur S2 et S3.

>![image](https://user-images.githubusercontent.com/95431446/170267722-1413422b-1b99-4208-b493-f13fc7584df8.png)
_Tout les vlan sont autorisé a traverser le trunk_

Etape 3 : 


