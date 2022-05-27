<p align="center">
<a href="[https://user-images.githubusercontent.com/95431446/169254026-e9b9e9d2-7027-4733-ae36-9c0ff3dd31d5.png](https://static.zerochan.net/Yor.Briar.full.3635982.gif)">
<img src="https://static.zerochan.net/Yor.Briar.full.3635982.gif"/>
</a>
</p>


# TP 1 Module 4

## Part 1 : configuration du protocole RIPv2

Etape 1 : configurez RIPv2 sur R1.

>![image](https://user-images.githubusercontent.com/95431446/170658029-060de6a1-689f-4f44-a7cd-e28abaf9e916.png)

Etape 2 : configurez RIPv2 sur R2.

>![image](https://user-images.githubusercontent.com/95431446/170659503-cbf4014e-fd86-4490-8c5b-d276efafa87c.png)

Etape 3 : configurez RIPv2 sur R3.

>![image](https://user-images.githubusercontent.com/95431446/170659968-9f37f424-1678-4198-8eef-e145e305677d.png)


# TP 2 Module 4

## Partie 1 : Ajout de VLAN à un commutateur

Etape 1 : création des réseaux locaux virtuels sur S1

>![image](https://user-images.githubusercontent.com/95431446/170662361-d754f6fe-f0a5-4fd9-a50e-82a6166cbd99.png)

Etape 3 : Test de la connectivité entre PC1 et PC3

À partir de PC1, envoyez une requête ping à PC3. Les requêtes ping doivent encore échouer. Pourquoi les requêtes ping n’ont-elles pas abouti ?

>![image](https://user-images.githubusercontent.com/95431446/170662544-df44d3ad-4e19-48b8-b802-b5d1b0ac8999.png)

## Partie 2 : Configuration des sous-interfaces

Étape 1 : Configurez des sous-interfaces sur R1 en utilisant l’encapsulation 802.1Q.

>![image](https://user-images.githubusercontent.com/95431446/170666558-e5679bfe-0f28-44a8-9391-ff6aab2e56e0.png)


>![image](https://user-images.githubusercontent.com/95431446/170667111-e8a91a9d-191d-4bf1-be9a-cd431a5fa3fe.png)

Etape 2 : Vérifiez la configuration.

A. Activez l’interface G0/0. Vérifiez que les sous-interfaces sont désormais actives.

>![image](https://user-images.githubusercontent.com/95431446/170670557-f9afe754-e657-4b14-b1f5-f09f94d94f06.png)

>![image](https://user-images.githubusercontent.com/95431446/170670610-e4a36b34-1081-49d2-83b5-98461552ace6.png)


## Partie 3 : Test de la connectivité avec routage inter-VLAN

Etape 1 : Requête ping entre PC1 et PC3

A partir de PC1, envoyez une requête ping à PC3. Les requêtes ping doivent encore échouer. Pourquoi ?

>Les trunks ne sont pas activé.

Etape 2 : Activez le trunking

Sur S1, exécutez la commande show vlan. À quel VLAN G0/1 est-elle attribuée ?

>VLAN 1 (default)

Activez le système de trunk sur l’interface G0/1.

>![image](https://user-images.githubusercontent.com/95431446/170672382-b7c80c89-8b08-414e-b740-44ba988bf328.png)


Comment déterminer si une interface est une ligne principale grâce à la commande show vlan ? 

>L’interface n’est plus répertoriée sous VLAN 1

Lancez la commande show interface trunk pour vérifier si l’interface a été configurée comme ligne 
principale.

>![image](https://user-images.githubusercontent.com/95431446/170672724-88335bc1-59e0-4593-89e8-5015fc239be2.png)




