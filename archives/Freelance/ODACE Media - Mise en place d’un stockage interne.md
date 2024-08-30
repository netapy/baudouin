> [!important]  
> ODACE Media a besoin de mettre en place un service de stockage interne pour stocker et partager les fichiers entre les membres de l’équipe.Par souci de praticité et d’indépendance, cette solution doit être hébergée dans les locaux de l’entreprise.  
# Besoin
- [ ] 100TB de stockage
- [ ] Hébergé dans les locaux
- [ ] Accès depuis n’importe quel appareil, n’importe où
# Solution
## **Software** : _NextCloud Files_
Parmi les différentes solutions du marché, NextCloud Files semble être la plus appropriée — elle est la plus stable, gratuite et backée par une entreprise importante.
NextCloud files fonctionne avec tous les systèmes d’exploitation et propose une interface en ligne (façon Google drive) pour uploaded/télécharger les fichiers.
## Hardware
NextCloud peut être installé sur pleins de serveurs différents, mais on privilégiera un hardware robuste extensible au besoin.
### Serveur
**Synology DS1621xs+**
- Synology a l’avantage d’avoir une gestion intelligente du RAID (sécurisation des données en cas de défaillance d’un disque) et à gérer beaucoup de paramètres automatiquement en fonction de l’utilisation.
- Environ 1100€
- 6 emplacements de disques durs (extensible à 16 avec un extender)
- Liens :
    
    > [!info] DiskStation® DS1621xs+ | Synology Inc.  
    > On-premises cloud solution built for performance  
    > [https://www.synology.com/en-uk/products/DS1621xs+](https://www.synology.com/en-uk/products/DS1621xs+)  
    
    > [!info]  
    >  
    > [https://www.darty.com/nav/achat/informatique/reseau/serveur_nas/synology_ds1621.html?store=907026&esl-k=sem-google%7Cng%7Cc240564131959%7Cm%7Ckpla1897125714479%7Cp%7Ct%7Cdc%7Ca49693353265%7Cg1019118428&dartycid=sea_shopping-local_LIA-ALL-Informatique_adgroup_Informatique&gclid=Cj0KCQiAorKfBhC0ARIsAHDzslsdYFDIGhP2c7KmXFcVd64k7vREgqMP1xDyoUwuzNBTp4QXShlYcN4aApv-EALw_wcB&gclsrc=aw.ds](https://www.darty.com/nav/achat/informatique/reseau/serveur_nas/synology_ds1621.html?store=907026&esl-k=sem-google%7Cng%7Cc240564131959%7Cm%7Ckpla1897125714479%7Cp%7Ct%7Cdc%7Ca49693353265%7Cg1019118428&dartycid=sea_shopping-local_LIA-ALL-Informatique_adgroup_Informatique&gclid=Cj0KCQiAorKfBhC0ARIsAHDzslsdYFDIGhP2c7KmXFcVd64k7vREgqMP1xDyoUwuzNBTp4QXShlYcN4aApv-EALw_wcB&gclsrc=aw.ds)  
    
### **Disques durs**
- A décider en fonction du budget et du terme souhaité.
- **HAT5300 Series 3.5” SATA HDD** (produit synology, plus fiable sur le long terme)
    - 12TB → 600€
    - 16TB → 800€
- **Seagate IronWolf Pro 3.5“** (produit pas dédié à cet usage, - fiable mais - cher)
    - 16TB → 350€
## Prochaines étapes:
- Évaluer les besoins en termes de stockage et décider du matériel à acheter ;
- Passer la commande du matériel ;
- Installer le serveur dans sa configuration de base ;
- Installer et configurer NextCloud files sur le serveur ;
- Test et déploiement de la solution.