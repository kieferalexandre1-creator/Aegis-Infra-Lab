# Aegis-Infra-Lab - Infrastructure d'Entreprise Sécurisée 
### 👤 Alexandre KIEFER
**Administrateur Systèmes, Réseaux & Cybersécurité**  
📍 Savigny-sur-Orge, Île-de-France  
🔗 [LinkedIn](https://www.linkedin.com/in/alexandre-kiefer-847334282/) | 🐙 [GitHub](https://github.com/kieferalexandre1-creator) | ✉️ kiefer.alexandre1@gmail.com

[![Statut](https://img.shields.io/badge/Statut-En%20d%C3%A9veloppement-orange)](#)
[![OS](https://img.shields.io/badge/Environnement-VirtualBox-blue)

## 📄 CV

Mon CV est disponible ici : 

[Accéder à mon dossier de candidature](https://drive.google.com/drive/folders/1oWsbNc7SqeIi7sD4AIL0xSP9bl1ns_SC?usp=drive_link)

## 👤 À propos de moi

Je travaille dans les domaines de l’administration systèmes, réseaux et cybersécurité, avec une première expérience professionnelle en support informatique, administration des systèmes et réseaux et sécurisation des infrastructures.

J’ai obtenu un **Titre Professionnel Technicien Informatique en 2024**, puis un **Bachelor Administrateur d’Infrastructures Sécurisées en 2025**.

J’ai commencé mon parcours avec un stage de trois mois chez **Kertios**, principalement autour du support informatique et de l’administration systèmes et réseaux. J’ai ensuite poursuivi avec environ un an d’alternance chez **Cesam Seed** en tant qu’Administrateur Systèmes, Réseaux & Cybersécurité.

Ces expériences m’ont permis de travailler sur des environnements Windows et Linux, la virtualisation avec VMware ESXi/vCenter, les réseaux, la sauvegarde, la supervision, la gestion des comptes et des droits d’accès ainsi que sur différents sujets liés à la sécurisation des infrastructures.

Je souhaite aujourd’hui poursuivre mon parcours professionnel sur des missions liées aux systèmes, aux réseaux, aux infrastructures IT et à la cybersécurité.

En parallèle, je développe **Aegis Infra Lab**, un laboratoire personnel conçu pour reproduire progressivement une infrastructure d’entreprise virtualisée et sécurisée. Ce projet me permet de continuer à pratiquer, tester différentes technologies et documenter concrètement les configurations, les choix techniques et les tests réalisés.

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

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/2d3db288-8ff5-40bb-ac7e-0c61f2e93d9b" />


## 🏗️ Architecture de l’infrastructure

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/de56d94f-fa52-4a39-a197-06e905f504b8" />

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

À ce stade du projet, les différentes machines du laboratoire utilisent un réseau Aegis commun afin de permettre les premiers déploiements et tests.

La configuration réseau actuellement utilisée est la suivante :

| Interface | Zone | Sous-réseau |
|---|---|---|
| WAN | Internet | NAT VirtualBox |
| LAN | Réseau Aegis | `192.168.56.0/24` |

Adresses principales utilisées actuellement :

- OPNsense LAN : `192.168.56.2`
- SRV-AEGISAD : `192.168.56.10`
- WIN-CLIENT01 : attribution DHCP à partir de `192.168.56.20`
- Plage DHCP : `192.168.56.20` à `192.168.56.50`

### Architecture cible

À terme, le laboratoire pourra être segmenté en plusieurs zones dédiées :

- Utilisateurs
- Infrastructure
- Services
- Supervision
- Sauvegarde

Cette évolution permettra de séparer davantage les postes, serveurs, services et sauvegardes afin de mieux contrôler les communications entre les différentes zones.

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

### 👥 Active Directory — OU, utilisateurs et groupes

Après le déploiement de Windows Server 2022, j’ai mis en place Active Directory afin de centraliser la gestion des utilisateurs, des groupes et des ordinateurs du domaine `aegis.local`.

L’objectif est de reproduire une organisation simple d’entreprise, avec une structure claire permettant ensuite d’appliquer des droits d’accès et des stratégies de groupe de manière ciblée.

La structure utilisée comprend notamment :

- une OU principale `AEGIS-ENTREPRISE` ;
- une OU `Utilisateurs` ;
- une OU `Groupes` ;
- une OU `Ordinateurs` ;
- une OU `Serveurs`.

Des groupes de sécurité ont également été créés pour représenter plusieurs services :

- `Informatique`
- `RH`
- `Comptabilite`

### 🗂️ Structure des unités d’organisation

L’arborescence Active Directory permet de séparer les différents types d’objets et de garder une organisation claire du domaine.

<img width="398" height="205" alt="Capture d&#39;écran 2026-09-28 173556" src="https://github.com/user-attachments/assets/8d803896-45bc-4eb9-9832-7362b1b77d79" />


Cette structure servira ensuite de base pour l’intégration des postes, l’application des GPO et la gestion des droits d’accès.

---

### ⚙️ Automatisation avec PowerShell

Une partie de la configuration Active Directory est automatisée avec PowerShell afin de rendre le déploiement plus rapide et reproductible.

Le script permet notamment de :

- créer l’OU principale `AEGIS-ENTREPRISE` ;
- créer les sous-OU ;
- créer les groupes de sécurité ;
- créer plusieurs utilisateurs de test ;
- affecter automatiquement les utilisateurs à leur groupe ;
- demander un mot de passe temporaire au moment de l’exécution.

<img width="944" height="716" alt="Capture d&#39;écran 2026-09-28 173525" src="https://github.com/user-attachments/assets/a4622450-8487-4978-8622-4fab1ea9f2b7" />

Le mot de passe n’est pas stocké directement dans le script : il est demandé au moment de l’exécution avec `Read-Host -AsSecureString`.

### 👤 Utilisateurs et groupes de sécurité

Des utilisateurs de test ont été créés afin de reproduire plusieurs profils présents dans une petite entreprise.

Chaque compte est rattaché à un groupe de sécurité correspondant à son service, ce qui permet ensuite de gérer plus facilement les droits d’accès et d’appliquer des règles adaptées.

Exemples de comptes utilisés dans le laboratoire :

- `jdupont` → groupe `Informatique`
- `cmartin` → groupe `RH`
- `tbernard` → groupe `Comptabilite`

<img width="151" height="121" alt="image" src="https://github.com/user-attachments/assets/9ad979a4-f7ba-40dd-ad95-446b90405a0d" />


Les groupes de sécurité permettent notamment de :

- centraliser la gestion des droits ;
- éviter d’attribuer des permissions directement à chaque utilisateur ;
- simplifier l’administration des accès ;
- préparer l’application de droits sur les dossiers, services et ressources réseau.

<img width="322" height="88" alt="image" src="https://github.com/user-attachments/assets/ea069b9c-ff0a-42b1-8534-35d554f74de5" />


Lors de la création des comptes, un mot de passe temporaire est attribué et l’utilisateur doit le modifier lors de sa première connexion.

### 🌐 DNS & DHCP

Windows Server 2022 assure également les services **DNS** et **DHCP** du laboratoire.

Ces deux rôles sont importants pour permettre aux postes clients de communiquer correctement sur le réseau et d’intégrer le domaine `aegis.local`.

#### 🌍 DNS

Le service DNS est utilisé pour résoudre les noms de machines et de services du domaine `aegis.local`.

Il joue un rôle important dans le fonctionnement d’Active Directory, notamment pour permettre aux postes clients de localiser le contrôleur de domaine et d’accéder aux différents services du laboratoire.

Une zone DNS dédiée au domaine `aegis.local` est configurée sur `SRV-AEGISAD`.

Le DNS permet notamment de :

- résoudre les noms des machines internes ;
- localiser le contrôleur de domaine ;
- assurer le bon fonctionnement d’Active Directory ;
- permettre aux postes clients d’accéder aux différents services du laboratoire.

Des tests de résolution sont ensuite réalisés depuis `WIN-CLIENT01`.

Le premier test permet de vérifier que le nom du serveur Active Directory est correctement résolu vers son adresse IP :

<img width="295" height="59" alt="Capture d&#39;écran 2026-09-29 151736" src="https://github.com/user-attachments/assets/654d10b7-9a78-4b70-8ea9-6624f5db2fae" />

Un second test permet de vérifier les enregistrements SRV utilisés par Active Directory pour localiser le contrôleur de domaine :

<img width="410" height="111" alt="Capture d&#39;écran 2026-09-29 153313" src="https://github.com/user-attachments/assets/fec133e4-bef1-4254-b163-fdf98c3647bc" />


#### 📡 DHCP

Le service DHCP est utilisé pour attribuer automatiquement les paramètres réseau aux postes clients du laboratoire.

Une étendue DHCP est configurée sur le réseau `192.168.56.0/24`.

La plage d’adresses distribuée est comprise entre `192.168.56.20` et `192.168.56.50`.

=
<img width="472" height="236" alt="image" src="https://github.com/user-attachments/assets/a51abb00-6d73-4118-b1f3-ef3cdf4a0157" />


Les options de l’étendue permettent ensuite de transmettre automatiquement les principaux paramètres réseau aux postes clients :

- passerelle par défaut : `192.168.56.2` ;
- serveur DNS : `192.168.56.10` ;
- suffixe DNS : `aegis.local`.
  
<img width="502" height="290" alt="image" src="https://github.com/user-attachments/assets/74126015-0e64-4932-8b7f-f451aa326082" />


Afin de vérifier le bon fonctionnement du service, `WIN-CLIENT01` est configuré pour obtenir automatiquement sa configuration réseau.

Le poste reçoit alors l’adresse `192.168.56.20`, ainsi que la passerelle et le suffixe DNS définis dans l’étendue.

<img width="323" height="127" alt="image" src="https://github.com/user-attachments/assets/19eb264f-c8f7-4a42-8f69-5bc53d159b07" />


Le bail attribué au poste client apparaît également dans la console DHCP du serveur.

<img width="855" height="257" alt="image" src="https://github.com/user-attachments/assets/e1be41b5-10dc-4901-886f-0f12c6214d4c" />

Ces tests permettent de confirmer que le serveur DHCP distribue correctement les paramètres réseau aux postes clients du laboratoire.

### 💻 Intégration du poste Windows au domaine

Une fois les services Active Directory, DNS et DHCP configurés, le poste `WIN-CLIENT01` est intégré au domaine `aegis.local`.

L’objectif est de permettre au poste client d’utiliser les comptes centralisés dans Active Directory et de recevoir les stratégies de groupe appliquées au domaine.

La jonction est réalisée en utilisant un compte administrateur du domaine.

Après l’intégration, le poste apparaît dans Active Directory comme objet ordinateur.

<img width="403" height="149" alt="image" src="https://github.com/user-attachments/assets/4808fda3-c574-46c1-b42f-dc68160964d7" />

Le poste est ensuite déplacé dans l’unité d’organisation dédiée aux ordinateurs du laboratoire afin de faciliter l’application des futures stratégies de groupe.

<img width="327" height="62" alt="image" src="https://github.com/user-attachments/assets/69e702f2-7f86-4e93-a74e-c17ff2c80a8c" />

### 👤 Connexion avec un utilisateur Active Directory

Après l’intégration du poste au domaine, une connexion est réalisée avec un compte utilisateur créé dans Active Directory.

Cette étape permet de vérifier que l’authentification centralisée fonctionne correctement et que le poste client utilise bien le contrôleur de domaine `SRV-AEGISAD`.

<img width="237" height="77" alt="image" src="https://github.com/user-attachments/assets/f080706c-637d-47c3-aa68-a9f7225efbd2" />

### 🔐 Stratégies de groupe — GPO

Les stratégies de groupe permettent de centraliser la configuration et la sécurisation des postes et des utilisateurs du domaine `aegis.local`.

Dans Aegis Infra Lab, les GPO sont utilisées pour appliquer automatiquement certaines règles aux utilisateurs et aux ordinateurs présents dans les différentes unités d’organisation.

L’objectif est de reproduire une administration centralisée proche d’un environnement d’entreprise, où les paramètres ne sont pas configurés manuellement poste par poste.

Plusieurs stratégies sont mises en place afin de tester différents types de configuration :

- restrictions utilisateur ;
- paramètres de sécurité ;
- configuration des postes ;
- application automatique de règles selon l’unité d’organisation.

#### 🚫 Restriction du Panneau de configuration

Une première stratégie de groupe est mise en place afin d’interdire l’accès au Panneau de configuration et aux paramètres Windows pour les utilisateurs concernés.

La GPO est liée à l’unité d’organisation `Utilisateurs`, ce qui permet de cibler les comptes présents dans cette OU.

Chemin de configuration :

<img width="831" height="529" alt="Capture d&#39;écran 2026-09-29 165338" src="https://github.com/user-attachments/assets/deb4ad0e-b452-4519-be17-e704cae84ef9" />

Après actualisation des stratégies sur le poste client, l’ouverture du Panneau de configuration est refusée pour l’utilisateur concerné.

<img width="473" height="270" alt="image" src="https://github.com/user-attachments/assets/4c667ee0-a4d4-474e-a4f5-5602da3bf991" />

Ce test confirme que la stratégie configurée sur le contrôleur de domaine est correctement appliquée au poste client.

#### 🔒 GPO de verrouillage automatique

Une seconde stratégie de groupe est mise en place afin de renforcer la sécurité des postes du domaine.

Cette GPO force le verrouillage automatique de la session après `300 secondes` d’inactivité.

Le paramètre configuré est le suivant :

<img width="544" height="228" alt="Capture d&#39;écran 2026-09-29 170516" src="https://github.com/user-attachments/assets/342be955-794a-40f3-bc9a-71451dfff933" />

Après application de la stratégie sur le poste client, la session se verrouille automatiquement lorsque la période d’inactivité définie est atteinte. 

Cette mesure permet de limiter les risques d’accès non autorisé à une session laissée ouverte sans surveillance.

<img width="510" height="401" alt="Capture d&#39;écran 2026-09-29 170543" src="https://github.com/user-attachments/assets/6b121a4e-4554-47e7-8a4e-0e9e927b417c" />

### 💾 Sauvegarde du serveur

Afin de protéger les services critiques du laboratoire, une sauvegarde du serveur `SRV-AEGISAD` est mise en place avec la fonctionnalité **Sauvegarde Windows Server**.

L’objectif est de disposer d’une copie du système permettant de récupérer les données et les composants du serveur en cas de problème.

Une sauvegarde complète du serveur est sélectionnée afin d’inclure les données, les applications ainsi que l’état du système.

<img width="324" height="280" alt="Capture d&#39;écran 2026-09-29 212508" src="https://github.com/user-attachments/assets/0632605e-0634-41b3-a268-564d82da34f0" />

La sauvegarde est stockée sur un volume dédié `E:`, séparé du disque système.

<img width="326" height="288" alt="Capture d&#39;écran 2026-09-29 212529" src="https://github.com/user-attachments/assets/b13a3fe3-393f-48a9-be47-fe0b0efcc271" />

Avant l’exécution, l’assistant permet de vérifier les différents éléments inclus dans la sauvegarde, notamment le disque système, l’état du système et les éléments nécessaires à une récupération complète.

La sauvegarde est ensuite exécutée et son résultat est contrôlé depuis la console Windows Server Backup.

<img width="1129" height="719" alt="Capture d&#39;écran 2026-09-29 213417" src="https://github.com/user-attachments/assets/52426e85-9eac-47a9-8abe-4ad184d9974f" />

La réussite de cette opération permet de valider la mise en place d’une première stratégie de protection du contrôleur de domaine et de ses services.

### ♻️ Test de restauration

Afin de vérifier que la sauvegarde est réellement exploitable, un test de restauration est réalisé sur un fichier volontairement supprimé.

Un fichier de test est créé sur le serveur, puis supprimé après l’exécution de la sauvegarde.

Depuis **Sauvegarde Windows Server**, l’assistant de récupération est utilisé afin de restaurer le fichier depuis la dernière sauvegarde disponible.

<img width="367" height="289" alt="image" src="https://github.com/user-attachments/assets/652dbb82-bccb-4cd9-a7e5-724b81babdb0" />

Le fichier est ensuite restauré à son emplacement d’origine.

<img width="395" height="303" alt="image" src="https://github.com/user-attachments/assets/890fd8d9-259b-4a78-a0c2-c9acdda97908" />

Ce test permet de confirmer que la sauvegarde réalisée est exploitable et que les données peuvent être récupérées en cas de suppression ou de problème.

### ✅ Bilan de l’environnement Windows

Cette première partie du laboratoire a permis de mettre en place et de valider les principaux services d’une infrastructure Windows d’entreprise.

Les éléments suivants ont été déployés et testés :

- Windows Server 2022 comme contrôleur de domaine ;
- Active Directory avec utilisateurs, groupes et unités d’organisation ;
- services DNS et DHCP ;
- intégration d’un poste Windows au domaine ;
- authentification avec un compte Active Directory ;
- application de stratégies de groupe (GPO) ;
- automatisation de certaines tâches avec PowerShell ;
- sauvegarde complète du serveur ;
- test de restauration des données.

Cette étape constitue la base de l’infrastructure Aegis Infra Lab et permet désormais d’intégrer progressivement les autres briques du projet, notamment Linux, les services web et la supervision.

## 🐧 Debian 12 & services Linux

Après la mise en place de l’environnement Windows, une machine Debian 12 est ajoutée au laboratoire afin d’intégrer une partie Linux à l’infrastructure.

L’objectif est de disposer d’un serveur Linux dédié à l’hébergement de services, à l’administration système et aux futurs tests de supervision et de sécurisation.

### 🏗️ Déploiement de Debian 12

Configuration prévue :

- Nom de la VM : `SRV-DEBIAN01`
- Système : Debian 12
- CPU : 2 vCPU
- Mémoire : 2 à 4 Go
- Stockage : 20 à 30 Go
- Adresse IP : `192.168.56.22/24`
- Passerelle : `192.168.56.2`
- DNS : `192.168.56.10`
  
🌐 Déploiement du serveur web NGINX

Afin d’ajouter un service web interne au laboratoire Aegis, j’ai installé NGINX sur le serveur Debian. L’objectif était d’héberger un portail technique centralisant les informations utiles à l’exploitation de l’infrastructure.
Après l’installation, le service a été activé au démarrage du système puis vérifié avec systemctl. Le statut active (running) confirme que NGINX fonctionne correctement sur le serveur.
La page par défaut de NGINX a ensuite été testée depuis un poste du réseau afin de vérifier que le service HTTP était bien accessible à distance.

<img width="598" height="395" alt="Capture d&#39;écran 2026-09-30 172247" src="https://github.com/user-attachments/assets/db39b389-d909-4613-82ac-26cba26275f8" />


🌐 Intégration au DNS interne

Pour éviter d’accéder au serveur web directement par son adresse IP, un enregistrement DNS de type A a été créé dans la zone aegis.local.
Le nom web.aegis.local permet ainsi d’accéder au portail NGINX depuis les machines utilisant le serveur DNS Active Directory.
Cette configuration permet d’intégrer le service Linux au reste de l’infrastructure et de conserver une résolution de noms centralisée.

<img width="371" height="263" alt="Capture d&#39;écran 2026-09-30 175639" src="https://github.com/user-attachments/assets/bd8fa447-9c24-4a80-afbd-83e3be6434e1" />

🖥️ Création du portail Aegis Internal Portal

La page NGINX par défaut a ensuite été remplacée par un portail technique interne développé pour le laboratoire.
Ce portail permet de centraliser plusieurs informations concernant l’infrastructure :
- environnement Windows ;
- réseau et pare-feu ;
- serveur Debian ;
- services web ;
- sauvegarde ;
- documentation ;
- sécurité ;
- protection des données.
  
L’objectif est de disposer d’une interface simple permettant de retrouver rapidement l’état et l’organisation des différents composants du laboratoire.

<img width="695" height="434" alt="Capture d&#39;écran 2026-09-30 184941" src="https://github.com/user-attachments/assets/e5f5c5a0-f1d9-46bd-9f48-f83e79e2ad00" />

📊 État des services

Une page dédiée à l’état des services a été ajoutée au portail afin d’obtenir une vue synthétique du serveur Debian.
Elle affiche notamment :

- le nom d’hôte ;
- l’adresse IP ;
- l’uptime ;
- l’utilisation du disque ;
- l’utilisation de la mémoire ;
- l’état du service NGINX ;
- l’état du service SSH ;
- le résultat de la résolution DNS Active Directory.
  
Les informations affichées sont générées à partir de l’état réel du serveur et ne sont pas simplement renseignées manuellement dans la page.

<img width="637" height="384" alt="Capture d&#39;écran 2026-09-30 184745" src="https://github.com/user-attachments/assets/07855c23-0a93-44f4-ba07-c783fe9e0260" />

⚙️ Automatisation de la mise à jour

La mise à jour de la page d’état est automatisée avec systemd.
Un timer exécute périodiquement le script chargé de récupérer les informations système et de régénérer la page de supervision légère du portail.
Cette automatisation permet de maintenir les informations à jour sans intervention manuelle et constitue une première approche de supervision avant le déploiement d’un outil dédié comme Zabbix.


🔐 Sécurité et contrôle des accès

Le portail comprend également une zone d’administration protégée par authentification.
Cette séparation permet de distinguer les informations générales du portail des zones réservées à l’administration.
Les journaux NGINX permettent également de conserver une trace des accès au serveur web et d’identifier d’éventuelles erreurs ou tentatives d’accès.


🛡️ Protection des données et principes RGPD

Une section dédiée à la protection des données a été ajoutée afin de documenter les bonnes pratiques appliquées dans le laboratoire.
Elle présente notamment :

- la minimisation des données ;
- l’utilisation d’identités fictives ;
- la gestion centralisée des accès ;
- le principe du moindre privilège ;
- la journalisation ;
- la sauvegarde ;
- la conservation limitée des informations.
- 
Cette section ne présente pas le laboratoire comme certifié conforme au RGPD. Elle permet plutôt de montrer comment certains principes de protection des données peuvent être intégrés à la conception et à l’exploitation d’une infrastructure.

<img width="956" height="461" alt="Capture d&#39;écran 2026-09-30 192717" src="https://github.com/user-attachments/assets/93673d25-e4f7-429c-bab8-6fbb899803a2" />

🧰 Suivi des incidents

Le portail contient une section consacrée aux incidents rencontrés pendant le déploiement.
Chaque incident peut être documenté avec :

- le problème constaté ;
- la cause identifiée ;
- les vérifications effectuées ;
- la résolution mise en œuvre ;
- le résultat final.
Les incidents liés à la jonction au domaine, à la résolution DNS et à la connectivité SSH ont par exemple été conservés afin de garder une trace des problèmes rencontrés et des solutions appliquées.

Cette partie permet également de montrer la démarche de diagnostic utilisée pendant le projet.

<img width="690" height="428" alt="Capture d&#39;écran 2026-09-30 191902" src="https://github.com/user-attachments/assets/e32f0ef2-8d78-4c5c-88e3-9e0a038ecc9b" />

📝 Journal des changements

Un journal des changements a été ajouté afin de suivre les principales évolutions du laboratoire.
Il permet de conserver une trace des déploiements et modifications importantes, comme :

- l’installation d’OPNsense ;
- le déploiement de Windows Server ;
- la jonction du poste client au domaine ;
- l’intégration de Debian à Active Directory ;
- le déploiement de NGINX ;
- la création du portail interne.
  
Chaque changement est associé à un objectif et à un état de validation.

<img width="639" height="241" alt="Capture d&#39;écran 2026-09-30 191949" src="https://github.com/user-attachments/assets/9ed7cb07-7a63-42a6-b866-dd7d3bf7f9af" />

✅ Bilan du déploiement NGINX

Le déploiement de NGINX a permis d’aller au-delà de la simple installation d’un serveur web.
Le serveur Debian héberge désormais un portail interne intégré à l’infrastructure Aegis, avec résolution DNS, état des services, automatisation avec systemd, documentation, suivi des incidents, journal des changements et prise en compte de plusieurs principes de sécurité et de protection des données.

Cette partie du projet permet de mettre en pratique l’administration Linux, les services web, le DNS, l’automatisation et la documentation technique au sein d’une même infrastructure.




