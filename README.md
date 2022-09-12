#INTRO BLOCKCHAIN

##Histoire de la blockchain ##
`présentation des diapos de Bernard BONCHE - cours électif de M1`

Problématiques : 
* authentification 
* certification 
* non falsification

Exemple de systeme 3 tiers (solution traditionnelle):   
un élève se connecte sur MyGes, authentification grâce à Google qui joue le rôle du tier de confiance. 


``Reseau Peer to peer : `` dans un réseau pair à pair, l'information est souvent décentralisée cad partout  la fois. Si un des noeuds tombe, il reste 99% de noeuds qui possèdent l'information.
Plus le nombre de noeuds augmente, plus la vitesse augmente car l'information est à plus d'endroits à la fois. (Emule,BitTorrent, PirateBay...) 

*Exemple de systeme décentralisé : Git* 

Principes : 
* partager l'information (données, base de données)
* validation de transaction (accord, traçage, immutabilité de la transaction)
* cryptographie (écrire, lire, modifier, supprimer selon les règles partagées et acceptées) : notions de clé privé (prouve la propriété en Blockchain) et publique  


###Instant culture générale ###
``Stuart Haber & Scott Stornetta (1991)`` : publication sur les premiers essais de la blockchain. Théorie d'un réseau décentralisé dans lequel les infos sont stockés dans des blocs (1 info/bloc)  
``Merkle Tree (1992)`` : permet de stocker plusieurs infos au sein d'un même bloc, optimise performances de la blockchain  
``Bitgold (2005)`` : décerner des titres de propriété dans la blockchain. Jeton qu'on pouvait dépenser deux fois (dépenser 1000€ sur son compte, et refaire la meme opération avant que le compte soit débité)``Double Spend`` Un jeton (token) = 1 élement avec un stock défini qu'on peut échanger de tier à tier dans un réseau décentralisé. Tous ces jetons sont identiques.  
``Bitcoin Whitepaper - Satoshi Nakamoto (2008)`` : préparer le code de la blockchain du bitcoin. Ce papier lance les fondements de la blockchain moderne.  
``Creation blockchain, prmeier déploiement Bitcoin(2009)``  

``Vitalik Buterin`` : Necessité de créer un langage adapté à la blockchain : création `` blockchain Etherium (2014)`` autour de laquelle on peut développer des application dApps (Decentralised Apps).  
3kM d'€ investis dans la blockchain

*NFT* : jeton unique, permet d'obtenir un certificat (ne peut pas servir de monnaie car unique). 


###Présentation de la blockchain ###

Un bloc = de l'information en liste chaînée.  
Un bloc : 
``  { id : 2 fois SHA256 (hexa)
    hash du bloc précédent (hexa)
    transaction : information } 
``  
La transaction a son propre hash. Elle est unique au sein d'un bloc. Plusieurs transaction dans un bloc.  

[Site etherscan](https://etherscan.io/) permet d'analyser les données du blockchain.

Dans un réseau décentralisé, un noeud doit contenir toutes les infos du réseau à un instant *t*. Un ``noeud léger`` contient une partie de l'information totale. La puissance de calcul est l'un des facteurs clé de la blockchain.  

Le processus de création de bloc = minage.   
``Mineur`` : personne qui alloue la puissance de calcul de sa carte graphique à la création d'un bloc.
Le but : calculer les hash des nouvelles transactions et des blocs.  
Problème : vérifier qu'à chaque nouveau bloc, tous les hash soient uniques à nouveau. En théorie, il y a un gap entre l'entrée de l'info dans la blockchain et la validation par les autres mineurs.

Les mineurs s'organisent en pool : un mineur mine un bloc, le pool est récompensé pour récompenser tous les mineurs. un pool plus puissant a plus de chances à offrir rémunération, mais cette rémunération sera divisée.  
##Solidity ##