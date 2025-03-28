# ARP Spoofing & DNS Sniffing Script
## Description :
Ce script Python utilise Scapy pour effectuer une attaque ARP Spoofing et intercepter les requêtes DNS sur un réseau local. Il redirige le trafic entre une cible et la passerelle, permettant ainsi à l'attaquant d'analyser les requêtes DNS envoyées par la victime.

## Fonctionnalités :
-  ARP Spoofing : Usurpe l'adresse MAC de la passerelle pour intercepter le trafic entre la victime et le routeur.
-   DNS Sniffing : Capture et affiche les requêtes DNS envoyées par les victimes sur le réseau.
-   Multi-threading : Exécution de l'attaque ARP en arrière-plan pendant la capture des paquets DNS.
##  Prérequis 
Avant d'exécuter le script, assurez-vous d'avoir :
- Python 3.x installé
- Scapy installé (pip install scapy)
- Privilèges administrateur (nécessaire pour envoyer des paquets ARP et capturer le trafic réseau)
## Installation 
Clonez le dépôt et installez les dépendances :
```bash
git clone https://github.com/Rizki033/ARP-Spoofing-DNS-Sniffing-Script.git
cd arp-dns-sniffer
pip install -r requirements.txt
```
## Utilisation
Exécutez le script avec les privilèges administrateur :
```bash
sudo python3 arp_dns_sniffer.py
```
Le script commencera à usurper l'adresse ARP et affichera les requêtes DNS interceptées.

## ⚠️  Avertissement
Ce script est strictement éducatif. Son utilisation sur un réseau sans autorisation est illégale. L'objectif est d'apprendre comment fonctionnent ces attaques pour mieux s'en protéger.

## 🛡 Comment se protéger ?
- Utiliser HTTPS : Crypte les requêtes DNS via DoH (DNS over HTTPS).
- Configurer un ARP Spoofing Detection : Outils comme Arpwatch peuvent alerter en cas d'attaque ARP.
- Activer DHCP Snooping : Empêche l'empoisonnement ARP sur certains réseaux.

