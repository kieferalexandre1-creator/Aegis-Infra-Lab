# Aegis-Infra-Lab - Infrastructure d'Entreprise Sécurisée 
### 👤 Alexandre KIEFER
**Administrateur Systèmes, Réseaux & Cybersécurité**  
📍 Savigny-sur-Orge, Île-de-France  
🔗 [LinkedIn](https://www.linkedin.com/in/alexandre-kiefer-847334282/) | 🐙 [GitHub](https://github.com/kieferalexandre1-creator) | ✉️ kiefer.alexandre1@gmail.com

[![Statut](https://img.shields.io/badge/Statut-En%20d%C3%A9veloppement-orange)](#)
[![OS](https://img.shields.io/badge/Environnement-VirtualBox-blue)

## 👤 À propos de moi

Je suis **junior en administration systèmes, réseaux et cybersécurité**, avec une première expérience professionnelle en support informatique, administration systèmes et réseaux et sécurisation des infrastructures.

J’ai obtenu un **Titre Professionnel Technicien Informatique en 2024**, puis un **Bachelor Administrateur d’Infrastructures Sécurisées en 2025**.

J’ai commencé mon parcours avec un stage de trois mois chez **Kertios**, principalement autour du support informatique et de l’administration systèmes et réseaux, avant de poursuivre avec environ un an d’alternance chez **Cesam Seed** en tant qu’Administrateur Systèmes, Réseaux & Cybersécurité.

Au fil de ces expériences, j’ai travaillé sur des environnements Windows et Linux, la virtualisation avec VMware ESXi/vCenter, les réseaux, la sauvegarde, la supervision, la gestion des comptes et des droits d’accès ainsi que sur différents sujets liés à la sécurisation des infrastructures.

Je souhaite aujourd’hui continuer à développer mes compétences sur des environnements systèmes, réseaux, infrastructures IT et cybersécurité.

En parallèle, je développe **Aegis Infra Lab**, mon laboratoire personnel. Il me permet de pratiquer en dehors du cadre professionnel, tester différentes technologies, construire progressivement une infrastructure complète et documenter concrètement les configurations et les tests réalisés.

---

## 💼 Expérience

- **≈ 1 an — Administrateur Systèmes, Réseaux & Cybersécurité**  
  Alternance — Cesam Seed

- **3 mois — Technicien Informatique**  
  Stage — Kertios

---

## 🎓 Formation

- **2025 — Bachelor Administrateur d’Infrastructures Sécurisées**  
  Niveau 6 — Bac+3

- **2024 — Titre Professionnel Technicien Informatique**  
  Niveau 5 — Bac+2

---

## 🏅 Certifications obtenues

- **Cisco — Network Technician Career Path**
- **AWS — Cloud Security Foundations**
- **Cisco — Junior Cybersecurity Analyst Career Path**

--

# 🛡️ Aegis Infra Lab

## 📌 Présentation du projet

Aegis Infra Lab est un projet personnel que j’ai créé pour mettre en pratique mes compétences en administration systèmes, réseaux et cybersécurité dans un environnement proche de celui d’une PME.

L’objectif est de construire progressivement une infrastructure complète et entièrement virtualisée afin de pouvoir installer, configurer, sécuriser, superviser et tester différents services sans dépendre d’un environnement de production.

Le laboratoire s’appuie principalement sur **VirtualBox, OPNsense, Windows Server 2022 et Debian 12**, avec l’intégration progressive de solutions de supervision, sauvegarde, automatisation et sécurité.

Chaque composant est installé, configuré, testé puis documenté avant de passer à l’étape suivante. Cette approche me permet de mieux comprendre le fonctionnement de l’infrastructure tout en conservant une trace claire des choix techniques et des résultats obtenus.

---

## 🎯 Objectifs du Lab

Aegis Infra Lab a pour objectif de reproduire progressivement une infrastructure informatique d’entreprise cohérente, sécurisée et documentée.

Le projet me permet notamment de :

- administrer des environnements **Windows et Linux** ;
- déployer et gérer un **Active Directory** ;
- administrer les **utilisateurs, groupes et droits d’accès** ;
- configurer les services **DNS et DHCP** ;
- intégrer des postes clients au domaine ;
- appliquer et tester des **GPO** ;
- segmenter les réseaux et contrôler les flux avec **OPNsense** ;
- sécuriser les communications entre les différentes zones ;
- mettre en place des services Linux avec **Debian** et **NGINX** ;
- superviser les systèmes et services avec **Zabbix** ;
- mettre en place une stratégie de **sauvegarde et de restauration** ;
- automatiser certaines tâches avec **PowerShell** et **Bash** ;
- centraliser et analyser progressivement les journaux système ;
- documenter chaque configuration, test et résultat obtenu.

L’objectif n’est pas uniquement d’installer des technologies, mais de comprendre leur rôle dans une infrastructure, de les faire fonctionner ensemble et de vérifier leur bon fonctionnement à travers des tests concrets.

---

## Environnement technique & choix technologiques

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/10154402-b84a-4c9c-8a7a-cc349484ec7e" />


## 🏗️ Architecture de l’infrastructure

Cette architecture présente l’organisation générale d’Aegis Infra Lab et la manière dont les différents systèmes, services et zones réseau interagissent entre eux.

L’objectif est de reproduire une infrastructure d’entreprise segmentée, dans laquelle les rôles sont séparés et les communications contrôlées par OPNsense.

<img width="1672" height="941" alt="image" src="https://github.com/user-attachments/assets/1f5c32b5-9bb7-4801-b1f1-5d5ed1db8903" />


L’infrastructure est organisée autour de plusieurs zones distinctes :

- **LAN Utilisateurs** : postes Windows intégrés au domaine ;
- **LAN Infrastructure** : Windows Server 2022, Active Directory, DNS, DHCP et GPO ;
- **Zone Services** : Debian 12, NGINX, Zabbix et autres services Linux ;
- **Zone Sauvegarde** : Veeam Backup & Replication et repository dédié.

OPNsense assure le routage, le filtrage et le contrôle des flux entre ces différentes zones.

## Sécurisation de l’infrastructure

La sécurité d’Aegis Infra Lab est intégrée progressivement à chaque couche de l’infrastructure.

L’objectif est de ne pas seulement protéger les machines individuellement, mais de mettre en place plusieurs niveaux de contrôle : réseau, systèmes, utilisateurs, services, supervision et sauvegarde.

### 🛡️ Principes de sécurité appliqués

<img width="1448" height="1086" alt="image" src="https://github.com/user-attachments/assets/a887f090-2806-4a12-861f-b3f742b2adcc" />

## 🔥 Déploiement d’OPNsense

OPNsense est la pièce centrale du réseau dans Aegis Infra Lab.

Je l’utilise comme **pare-feu et routeur** pour relier les différentes zones du laboratoire, contrôler les flux entre elles et gérer l’accès à Internet.

L’objectif est d’éviter que toutes les machines puissent communiquer librement entre elles, et de pouvoir définir précisément quels échanges sont autorisés ou bloqués selon les besoins.

---

### 🖥️ Déploiement de la machine virtuelle

OPNsense est installé dans une machine virtuelle dédiée sous VirtualBox.

Configuration utilisée :

- **Nom de la VM :** `OPNsense-FW`
- **Système :** FreeBSD 64-bit
- **CPU :** 2 vCPU
- **Mémoire :** 4 Go
- **Stockage :** 20 à 32 Go
- **Interface WAN :** NAT
- **Interfaces internes :** réseaux VirtualBox dédiés aux différentes zones du laboratoire

L’interface WAN permet à OPNsense d’accéder à Internet via la connexion réseau de la machine hôte.

Les autres interfaces sont utilisées pour connecter les différentes zones du laboratoire.

<img width="374" height="206" alt="Capture d&#39;écran 2026-09-21 215815" src="https://github.com/user-attachments/assets/9d9e51c9-ab7a-4ed0-8270-0535b833a2c1" />


---

### 🌐 Interface Web d’administration

Une fois OPNsense installé et les interfaces réseau configurées, l’administration du pare-feu est réalisée depuis son interface Web.

Le tableau de bord permet d’avoir une vue rapide sur l’état du système, les services actifs, les passerelles ainsi que les interfaces LAN et WAN.

<img width="225" height="227" alt="Capture d&#39;écran 2026-09-22 203011" src="https://github.com/user-attachments/assets/c5223775-27a3-48e5-9b76-7d4370290d0c" />


---

### 📌 Pourquoi OPNsense est important dans le projet

J’ai choisi OPNsense pour avoir un point central capable de gérer les communications entre les différentes zones du laboratoire.

Il me permet de travailler concrètement sur :

- le routage entre les sous-réseaux ;
- la création de règles de pare-feu ;
- le filtrage des flux entre les zones ;
- la séparation des postes, serveurs et services ;
- le principe du moindre privilège ;
- la journalisation des communications ;
- les tests de flux autorisés et bloqués.

L’intérêt est surtout de pouvoir reproduire une logique proche d’une infrastructure d’entreprise, où les machines ne communiquent pas toutes librement entre elles et où chaque accès doit répondre à un besoin précis.

---


### 🗺️ Schéma du rôle d’OPNsense

Le schéma suivant présente la place d’OPNsense au sein du laboratoire et les différentes zones réseau qu’il contrôle.

<img width="1312" height="1199" alt="Schéma du rôle d'OPNsense dans Aegis Infra Lab" src="https://github.com/user-attachments/assets/bcdf33cb-8f2e-4bcc-a655-fa13c91ad6d0" />

---

### 🌐 Segmentation réseau

Chaque zone du laboratoire dispose de son propre sous-réseau afin de séparer les usages et de mieux contrôler les communications entre les différents équipements.

Le découpage prévu est le suivant :

| Interface | Zone | Sous-réseau |
|---|---|---|
| WAN | Internet | NAT VirtualBox |
| LAN 1 | Utilisateurs | `192.168.10.0/24` |
| LAN 2 | Infrastructure | `192.168.20.0/24` |
| LAN 3 | Services | `192.168.30.0/24` |
| LAN 4 | Sauvegarde | `192.168.40.0/24` |

Ce découpage permet de séparer les postes clients, les serveurs, les services et les sauvegardes afin d’éviter qu’ils puissent communiquer librement entre eux.

---

### 🔌 Interfaces réseau

OPNsense est chargé de relier ces différentes zones et d’appliquer les règles de filtrage associées à chaque interface.

À ce stade du projet, la configuration est mise en place progressivement. Les sous-réseaux et interfaces pourront être ajustés au fur et à mesure de l’évolution du laboratoire.

<img width="1280" height="355" alt="Capture d&#39;écran 2026-09-22 203306" src="https://github.com/user-attachments/assets/02062444-51a2-471f-95a3-b90ada471e0e" />

---

### 🔐 Filtrage réseau

Les règles de pare-feu sont mises en place afin d’appliquer une logique de **moindre privilège**.

L’objectif est de n’autoriser que les communications réellement nécessaires au fonctionnement de l’infrastructure.

Quelques exemples de règles prévues ou mises en place :

- autoriser les postes utilisateurs à accéder à Internet ;
- limiter l’accès des postes utilisateurs aux serveurs ;
- autoriser uniquement les services nécessaires vers Windows Server ;
- permettre à Zabbix de superviser les serveurs et équipements ;
- empêcher l’accès direct des utilisateurs à la zone de sauvegarde ;
- limiter les communications entre les différentes zones ;
- bloquer les flux qui ne sont pas explicitement autorisés.

<img width="1026" height="498" alt="Capture d&#39;écran 2026-09-22 201459" src="https://github.com/user-attachments/assets/4588ae7a-b9eb-4bd8-ad44-b2814caa520a" />

### ✅ Validation d’un flux autorisé

Un premier test a été réalisé afin de vérifier qu’un trafic légitime pouvait traverser correctement le pare-feu.

Les journaux OPNsense affichent plusieurs entrées avec l’action :

`pass`

Cela confirme que les communications correspondant aux règles autorisées sont bien prises en compte et journalisées par le pare-feu.

<img width="377" height="209" alt="Capture d&#39;écran 2026-09-22 200824 - Copie" src="https://github.com/user-attachments/assets/67f81f02-2bf9-4556-93a7-224255b771ec" />

Cette étape permet de vérifier que les flux nécessaires au fonctionnement de l’infrastructure ne sont pas bloqués.

Cette approche permet de réduire la surface d’attaque et de limiter les mouvements possibles en cas de compromission d’une machine.

### ⛔ Validation d’un flux bloqué

Un second test a été réalisé afin de vérifier qu’une règle de blocage personnalisée était bien appliquée.

Le trafic provenant du réseau LAN a volontairement été dirigé vers un service dont l’accès devait être refusé.

Les journaux OPNsense font apparaître plusieurs événements associés à la règle :

`USER_RULE: Block LAN to Services`

<img width="1026" height="498" alt="Capture d&#39;écran 2026-09-22 201459" src="https://github.com/user-attachments/assets/5208f4c7-e05b-401b-901a-07a3a2f1c2de" />


Cette capture confirme que le trafic concerné est bien identifié, bloqué puis journalisé par OPNsense.

Ce test permet de valider le bon fonctionnement du filtrage mis en place entre les différentes zones du laboratoire.

### ✅ Bilan de la configuration OPNsense

Cette étape m’a permis de mettre en place la première brique réseau du laboratoire et de vérifier son fonctionnement dans des conditions concrètes.

J’ai pu notamment :

- déployer OPNsense dans une machine virtuelle dédiée ;
- configurer les interfaces WAN et LAN ;
- accéder à l’interface Web d’administration ;
- mettre en place des règles de filtrage ;
- autoriser certains flux nécessaires ;
- bloquer des communications non autorisées ;
- vérifier les résultats dans les journaux du pare-feu.

OPNsense servira de base pour la suite du projet, notamment pour la segmentation complète des différentes zones et le contrôle des communications entre les postes, les serveurs, les services et la zone de sauvegarde.

## 🖥️ Windows Server & Active Directory

### 🏗️ Déploiement de Windows Server 2022

Windows Server 2022 constitue la base de l’environnement Microsoft d’Aegis Infra Lab.

Je l’utilise pour centraliser les principaux services d’infrastructure du laboratoire, notamment **Active Directory, DNS, DHCP et les stratégies de groupe (GPO)**.

L’objectif est de reproduire un environnement proche de celui d’une entreprise, avec une gestion centralisée des utilisateurs, des postes et des ressources.

La machine est déployée dans VirtualBox avec une configuration dédiée au laboratoire.

Configuration utilisée :

- **Nom de la VM :** `WIN-SRV-AD01`
- **Système :** Windows Server 2022
- **Rôle principal :** contrôleur de domaine
- **Domaine :** `aegis.local`
- **Adresse IP :** `192.168.56.10/24`
- **Passerelle :** `192.168.56.2`
- **DNS :** `192.168.56.10`

Les rôles principaux installés sont :

- **Active Directory Domain Services (AD DS)** ;
- **DNS** ;
- **DHCP** ;
- **Services de fichiers et de stockage**.

### 🧩 Rôles installés

Le Gestionnaire de serveur permet de vérifier rapidement les différents rôles actuellement déployés sur la machine.

<img width="1620" height="703" alt="image" src="https://github.com/user-attachments/assets/8be086e8-0ebf-475c-8962-b8a6b95d83e0" />


Cette configuration permet au serveur de centraliser l’authentification, la résolution DNS et l’attribution des paramètres réseau aux différentes machines du laboratoire.

---

### 🌐 Configuration réseau du serveur

Le contrôleur de domaine utilise une adresse IP fixe afin de rester joignable de manière constante par les postes clients et les différents services du laboratoire.

<img width="391" height="450" alt="image" src="https://github.com/user-attachments/assets/795167c2-74c9-4bfc-8531-274bc439dd70" />

La passerelle correspond à l’interface LAN d’OPNsense, tandis que le serveur utilise son propre service DNS pour la résolution du domaine `aegis.local`.

---

### 🏢 Domaine Active Directory

Le domaine Active Directory utilisé dans Aegis Infra Lab est :

`aegis.local`

<img width="352" height="219" alt="image" src="https://github.com/user-attachments/assets/457d874b-d863-4422-b6db-5572d74f1f49" />


Ce domaine servira ensuite à intégrer les postes Windows, centraliser les comptes utilisateurs, gérer les groupes et appliquer les stratégies de groupe.
