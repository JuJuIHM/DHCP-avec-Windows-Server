# DHCP-avec-Windows-Server
DHCP avec Windows Server

Il y a 2 façons de réaliser l'installation des rôles DHCP sur le serveur, avec gestionnaire de serveur ou Power Shell.

Tout d'abord changer le nom du serveur
![Photo](https://ibb.co/68fy54g)

**Environnement virtuel**
SRVW12_Q1 : serveur Windows 12 qui fait office de serveur DHCP
DESKTOP-R04V9QR Windows 10 : client DHCP

# Installation des rôles

Définir une IP static à SRVW12_Q1
Aller dans serveur local et cliquer sur Adresse IPv4 attribuée par DHCP
![Photo](https://ibb.co/N23wFWm)

Cliquer sur Ethernet, puis propriétés et protocole Internet version 4
![Photo](https://ibb.co/1TFfw28)

Définir une plage d'adresses IP à attribuer
![Photo](https://ibb.co/nk5MtQg)
*erreur sur adresse IP de la copie écran

Cliquer sur Gérer, puis installer un rôle une fonctionnalité.
Sélectionner un type d'installation 
![Photo](https://ibb.co/jHMvfCW)

Sélectionner le serveur 
![Photo](https://ibb.co/f8k2gn9)

Sélectionner fonctionnalités et cocher serveur DHCP
![Photo](https://ibb.co/nzBgpfj)

![Photo](https://ibb.co/VmK8k4F)

![Photo](https://ibb.co/vPjXKnv)

![Photo](https://ibb.co/0JK2v2V)

Récupérer l'adresse MAC de DESKTOP-R04V9QR Windows 10 : client DHCP
![Photo](https://ibb.co/4RFHtLr)
Adresse MAC : 08-00-27-F1-5E-91

# Gestion du serveur DHCP

Menu démarrer, puis outils d'administration et Console DHCP
![Photo](https://ibb.co/kGpRJWN)

Ajouter une étendue
![Photo](https://ibb.co/kccKmDF)

![Photo](https://ibb.co/N3LWXV1)

![Photo](https://ibb.co/X7tVR2N)
*Erreur dans adresse IP de début => corection : 192.168.1.201

# Nouvelle réservation 

![Photo](https://ibb.co/QYYvY6m)

![Photo](https://ibb.co/yh6Mnf4) 

![Photo](https://ibb.co/9HyZYP8)













