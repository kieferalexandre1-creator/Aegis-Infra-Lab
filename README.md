# Aegis-Infra-Lab - Infrastructure d'Entreprise Sécurisée 
### 👤 Alexandre KIEFER
**Administrateur Systèmes, Réseaux & Cybersécurité**  
📍 Savigny-sur-Orge, Île-de-France  
🔗 [LinkedIn](https://www.linkedin.com/in/alexandre-kiefer-847334282/) | 🐙 [GitHub](https://github.com/kieferalexandre1-creator) | ✉️ kiefer.alexandre1@gmail.com

[![Statut](https://img.shields.io/badge/Statut-En%20d%C3%A9veloppement-orange)](#)
[![OS](https://img.shields.io/badge/Environnement-VirtualBox-blue)](#)

## Présentation du Projet
Ce projet a pour objectif la conception, le déploiement et le durcissement complet d'une infrastructure réseau et système pour une PME fictive.
L'environnement est entièrement virtualisé sous **VirtualBox** et intègre la segmentation réseau, la gestion centralisée des identités, le contrôle des accès et la supervision.

## Topologie Réseau
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/0b1654d6-e73d-4eed-b582-e3c65ae153f5" />

## 🛠️ Briques Techniques & Composants
* **Pare-feu & Routage :** OPNsense (Segmentation VLAN, règles de filtrage ACL, VPN)
* **Identity & Annuaire :** Windows Server 2022 (Active Directory DS, DNS, GPO de durcissement)
* **Services Linux :** Debian 12 (Reverse Proxy NGINX avec certificats SSL/TLS)
* **Supervision & Log :** Zabbix Server & Agents
* **Sauvegarde :** Stratégie 3-2-1
* **Automatisation :** Scripts PowerShell (gestion AD) et Bash

## Fonctionnalités & Sécurisation Mises en Œuvre
### 🔐 1. Sécurité Réseau
- Isolation des flux via segmentation.
- Blocage par défaut du trafic inter-zones (Principe du moindre privilège).

### 🏢 2. Administration Système & Identity
- Déploiement du domaine `aegis.local`.
- Organisation de l'annuaire via Unités d'Organisation (OU) par service.
- Application de GPO pour le durcissement du pare-feu local et le verrouillage des sessions.

### 📊 3. Monitoring & MCO
- Surveillance en temps réel de la disponibilité et des ressources (CPU/RAM/Disque).
