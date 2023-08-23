# DHCP-avec-Windows-Server


*Les IP utilisées dans ce cas pratique ne sont pas les mêmes que celui de l'énoncé.

Il y a 2 façons de réaliser l'installation des rôles DHCP sur le serveur, avec gestionnaire de serveur ou Power Shell.

**Environnement virtuel**

SRVW12_Q1 : serveur Windows 12 qui fait office de serveur DHCP

DESKTOP-R04V9QR Windows 10 : client DHCP


Tout d'abord changer le nom du serveur

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/b723043c-5025-4b1e-a46d-4ce40f6807c0)


# Installation des rôles

Définir une IP static à SRVW12_Q1

Aller dans serveur local et cliquer sur Adresse IPv4 attribuée par DHCP

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/e5d4a8b6-a0d1-4f80-83d8-5853a619d56c)

Cliquer sur Ethernet, puis propriétés et protocole Internet version 4

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/04a692be-d500-432d-aa70-4ce54635087e)


Définir une plage d'adresses IP à attribuer

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/9a6354dc-fc07-461a-8afa-1842e33441ea)

*erreur sur adresse IP de la copie écran

Cliquer sur Gérer, puis installer un rôle une fonctionnalité.

Sélectionner un type d'installation 

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/ed1af6f1-1e65-448f-a246-4a52cda310b0)

Sélectionner le serveur 

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/02856058-9229-44e4-af07-e852f06f7982)

Sélectionner fonctionnalités et cocher serveur DHCP

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/01ec449a-04cb-4b75-bcc4-a13d3513b986)

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/4e2e7455-fd10-42ef-abe5-5dce9627bc68)

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/e2cbebc4-91dd-4a8c-a2a0-183d05e1450b)

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/17e54514-5c35-4f8e-a270-4c45021cdf5f)


Récupérer l'adresse MAC de DESKTOP-R04V9QR Windows 10 : client DHCP

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/468d4b8e-6726-4ae3-a9f3-24480017d272)

Adresse MAC : 08-00-27-F1-5E-91

# Gestion du serveur DHCP

Menu démarrer, puis outils d'administration et Console DHCP

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/4cd2268b-c072-4636-810c-fe744d0839cc)


Ajouter une étendue

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/46d89b1a-a94c-4ec2-b35e-193dc983bb6d)


![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/75fd6311-e8d3-4c21-b1ca-cdf16265e4ab)

*Erreur dans adresse IP de début => corection : 192.168.1.201

# Nouvelle réservation 


![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/d8330609-cee6-485f-bda0-47ec5f1aeb8b)

![image](https://github.com/JuJuIHM/DHCP-avec-Windows-Server/assets/137881830/f2fd02bf-5738-42f8-ac11-171c42d38d39)

![Photo](https://i.ibb.co/QvYDm0b/Screenshot-2023-08-22-IPHost1.png)













