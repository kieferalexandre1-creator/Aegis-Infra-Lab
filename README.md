# Aegis-Infra-Lab - Infrastructure d'Entreprise Sécurisée 
### 👤 Alexandre KIEFER
**Administrateur Systèmes, Réseaux & Cybersécurité**  
📍 Savigny-sur-Orge, Île-de-France  
🔗 [LinkedIn](https://www.linkedin.com/in/alexandre-kiefer-847334282/) | 🐙 [GitHub](https://github.com/kieferalexandre1-creator) | ✉️ kiefer.alexandre1@gmail.com

[![Statut](https://img.shields.io/badge/Statut-En%20d%C3%A9veloppement-orange)](#)
[![OS](https://img.shields.io/badge/Environnement-VirtualBox-blue)

## 👤 À propos de moi

Profil junior en systèmes, réseaux et cybersécurité, j’ai obtenu un Titre Professionnel Technicien Informatique en 2024, puis un Bachelor Administrateur d’Infrastructures Sécurisées en 2025.

J’ai commencé mon parcours avec un stage de 3 mois chez Kertios, principalement autour du support informatique et de l’administration systèmes et réseaux. J’ai ensuite réalisé environ un an d’alternance chez Cesam Seed en tant qu’Administrateur Systèmes, Réseaux & Cybersécurité.

Ces expériences m’ont permis de travailler sur des environnements Windows et Linux, la virtualisation avec VMware ESXi/vCenter, les réseaux, la sauvegarde, la supervision, la gestion des comptes et des droits d’accès, ainsi que sur différents sujets liés à la sécurisation des infrastructures.

Je souhaite aujourd’hui continuer à progresser dans ces domaines et poursuivre mon parcours avec un Mastère Expert Cybersécurité en alternance.

J’ai créé Aegis Infra Lab pour continuer à pratiquer en dehors du cadre professionnel, tester différentes technologies, construire une infrastructure complète et documenter concrètement les étapes de mon travail.

---

## 💼 Expérience

- **≈ 1 an — Administrateur Systèmes, Réseaux & Cybersécurité**  
  Alternance

- **3 mois — Technicien Informatique**  
  Stage

---

## 🎓 Formation

- **2025 — Bachelor Administrateur d’Infrastructures Sécurisées**  
  Niveau 6 — Bac+3

- **2024 — Titre Professionnel Technicien Informatique**  
  Niveau 5 — Bac+2

- **Projet 2026 — Mastère Expert Cybersécurité**  
  Recherche d’une alternance de 2 ans

---

## 🎯 Postes recherchés

Je recherche principalement des opportunités junior en :

- Administration Systèmes & Réseaux
- Administration d’infrastructures IT
- Systèmes, Réseaux & Sécurité
- Cybersécurité des infrastructures
- Technicien Cybersécurité
- Analyste SOC Junior
- Support Informatique N1/N2

---

## 🏅 Certifications obtenues

- **Cisco — Network Technician Career Path**
- **AWS — Cloud Security Foundations**
- **Cisco — Junior Cybersecurity Analyst Career Path**

---

## 📚 Certifications visées

- **CompTIA Security+**
- **eJPT — Junior Penetration Tester**
- **CRTP — Certified Red Team Professional**


---

# Aegis Infra Lab

## 📌 Présentation du projet

**Aegis Infra Lab** est un laboratoire personnel conçu pour reproduire l’infrastructure informatique d’une PME fictive dans un environnement entièrement virtualisé.

L’objectif est de construire progressivement une infrastructure permettant de mettre en pratique plusieurs compétences liées à l’**administration systèmes et réseaux**, à la **sécurisation des infrastructures**, à la **supervision** et à l’**automatisation**.

Le laboratoire repose principalement sur **VirtualBox**, **OPNsense**, **Windows Server 2022** et **Debian 12**.

Le projet est développé progressivement afin de pouvoir configurer, tester et documenter chaque composant avant d’intégrer de nouvelles fonctionnalités.

---

## 🎯 Objectifs du Lab

Aegis Infra Lab a pour objectif de mettre en pratique :

- l’administration de systèmes Windows et Linux ;
- le déploiement et l’administration d’Active Directory ;
- la gestion des utilisateurs, groupes et droits d’accès ;
- les services DNS et DHCP ;
- la segmentation et le filtrage réseau ;
- l’administration d’un pare-feu OPNsense ;
- la sécurisation des systèmes et des services ;
- la supervision des équipements et serveurs ;
- l’automatisation de tâches d’administration ;
- la sauvegarde et la continuité de service.

---

## Environnement technique

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/89df2a9c-84b7-4425-864f-4a3ee7357820" />



## 🏗️ Architecture de l’infrastructure

L’infrastructure est organisée autour d’un pare-feu **OPNsense**, chargé du routage et du contrôle des communications entre les différentes zones du laboratoire.

Elle comprend progressivement :

- un environnement **Windows Server 2022** pour Active Directory, DNS et DHCP ;

- des postes clients Windows intégrés au domaine ;

- un serveur **Debian 12** pour différents services Linux ;

- une solution de supervision ;

- différentes zones réseau séparées et contrôlées par OPNsense.

### Schéma de l’architectur

## 🔐 Sécurisation de l’infrastructure

Plusieurs principes de sécurité sont progressivement appliqués au laboratoire :

- segmentation des différentes zones réseau ;

- filtrage des communications entre les zones ;

- principe du moindre privilège ;

- gestion centralisée des utilisateurs et des groupes ;

- contrôle des droits d’accès ;

- durcissement des systèmes Windows via GPO ;

- sécurisation des services Linux ;

- utilisation de certificats SSL/TLS ;

- supervision des systèmes et services ;

- journalisation des événements.

---

## 🔥 Déploiement d’OPNsense

OPNsense constitue la première brique réseau d’Aegis Infra Lab.

Il est utilisé comme **pare-feu et routeur principal** afin de gérer le routage, la segmentation et le filtrage des communications entre les différentes zones du laboratoire.

Son rôle est central dans le projet, car l’ensemble des réseaux internes transitent par OPNsense avant de pouvoir communiquer entre eux ou accéder à Internet.

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

Les autres interfaces seront utilisées pour connecter les différentes zones du laboratoire.

---

### 📌 Importance d’OPNsense dans le projet

OPNsense se situe au cœur de l’architecture Aegis Infra Lab.

Il permet notamment de :

- relier les différents réseaux ;
- assurer le routage entre les sous-réseaux ;
- contrôler les communications entre les zones ;
- appliquer des règles de pare-feu ;
- segmenter les postes clients, les serveurs et les services ;
- limiter les flux au strict nécessaire ;
- isoler les services sensibles ;
- appliquer le principe du moindre privilège ;
- journaliser les communications ;
- tester des scénarios de sécurité réalistes.

Sans cette segmentation, les différentes machines du laboratoire pourraient communiquer librement entre elles, ce qui ne correspondrait pas à une architecture d’entreprise sécurisée.

---

### 🗺️ Schéma du rôle d’OPNsense

Le schéma suivant présente la place d’OPNsense au sein du laboratoire et les différentes zones réseau qu’il contrôle.

<img width="1312" height="1199" alt="image" src="https://github.com/user-attachments/assets/bcdf33cb-8f2e-4bcc-a655-fa13c91ad6d0" />
---

### 🌐 Segmentation réseau

L’infrastructure est progressivement séparée en plusieurs zones.

<img width="1916" height="821" alt="image" src="https://github.com/user-attachments/assets/fcbaef27-fadc-46cb-8675-7561c3fb7b49" />


Chaque zone dispose de son propre sous-réseau et de règles de filtrage adaptées à son rôle.

🔌 Interfaces réseau prévues

Le découpage prévu est le suivant :

Interface	Zone	Sous-réseau
WAN	Internet	NAT VirtualBox
LAN 1	Utilisateurs	192.168.10.0/24
LAN 2	Infrastructure	192.168.20.0/24
LAN 3	Services	192.168.30.0/24
LAN 4	Sauvegarde	192.168.40.0/24

Les adresses pourront être adaptées au fur et à mesure de la configuration du laboratoire.

🔐 Filtrage réseau

Les règles de pare-feu seront progressivement mises en place afin d’appliquer une logique de moindre privilège.

Quelques exemples de règles prévues :

autoriser les postes utilisateurs à accéder à Internet ;
limiter l’accès des postes utilisateurs aux serveurs ;
autoriser uniquement les services nécessaires vers Windows Server ;
autoriser Zabbix à superviser les serveurs et équipements ;
empêcher l’accès direct des utilisateurs à la zone de sauvegarde ;
limiter les communications entre les différentes zones ;
bloquer les flux non explicitement autorisés.

L’objectif est de réduire la surface d’attaque et d’éviter qu’une machine compromise puisse communiquer librement avec l’ensemble de l’infrastructure.

🧪 Tests de validation

La configuration d’OPNsense sera validée avec différents tests.

Les tests comprendront notamment :

vérification du fonctionnement de l’interface WAN ;
vérification de l’accès à Internet ;
vérification des interfaces internes ;
accès à l’interface Web d’administration ;
test de connectivité avec les différentes machines ;
test du routage entre les réseaux ;
test des règles de pare-feu ;
test d’un flux explicitement autorisé ;
test d’un flux explicitement bloqué ;
vérification des journaux OPNsense.

Les résultats seront documentés avec des captures d’écran.

📸 Captures prévues

Les captures OPNsense seront enregistrées dans :

screenshots/opnsense/

Les principales captures prévues sont :

console OPNsense après installation ;
interfaces WAN et LAN ;
tableau de bord Web ;
attribution des interfaces ;
règles de pare-feu ;
segmentation des réseaux ;
test d’un flux autorisé ;
test d’un flux bloqué ;
journaux du pare-feu.

Exemples de fichiers :

screenshots/opnsense/
├── installation-console.png
├── interfaces.png
├── dashboard.png
├── firewall-rules.png
├── allowed-traffic-test.png
├── blocked-traffic-test.png
└── firewall-logs.png
📌 État de cette étape

🚧 Configuration en cours

L’installation de la machine virtuelle OPNsense est actuellement en cours.

Les prochaines étapes seront :

finaliser l’installation ;
attribuer les interfaces réseau ;
configurer l’accès à l’interface Web ;
créer les différentes zones ;
attribuer les sous-réseaux ;
mettre en place les premières règles de filtrage ;
effectuer les tests de connectivité ;
documenter les résultats obtenus.


``


Et la ligne qui l’affiche est déjà placée au bon endroit dans le bloc :
## ⚙️ Automatisation

Certaines tâches d’administration sont automatisées afin de rendre le laboratoire plus facilement reproductible.

L’automatisation concerne notamment :

- la création de l’arborescence Active Directory ;

- la création des unités d’organisation (OU) ;

- la création des groupes de sécurité ;

- le provisioning des utilisateurs ;

- l’affectation des utilisateurs aux groupes ;

- différentes tâches d’administration Windows via PowerShell.

Les scripts seront disponibles dans le dossier : 

## 🛠️ Automatisation Active Directory (`Deploy-AegisAD.ps1`)

Le déploiement de l'arborescence, des groupes de sécurité et des utilisateurs du domaine `aegis.local` est entièrement automatisé via le script PowerShell `Deploy-AegisAD.ps1`.

### 📌 Fonctionnalités du script
* **Structure d'OU** : Création de l'OU racine `AEGIS-ENTREPRISE` et des sous-OU (`Utilisateurs`, `Groupes`, `Ordinateurs`, `Serveurs`).
* **Groupes de sécurité** : Création des groupes globaux par service (`GRP_Informatique`, `GRP_Ressources-Humaines`, `GRP_Comptabilite`).
* **Provisioning Utilisateurs** : Création des comptes avec identifiants normalisés (`jdupont`, `cmartin`, `tbernard`), mot de passe temporaire et réinitialisation obligatoire à la première connexion.
* **Gestion des membres** : Affectation automatique de chaque utilisateur à son groupe respectif.

## ⚙️ Automatisation PowerShell

Une partie de la configuration Active Directory est automatisée avec PowerShell.

Le script permet notamment de :

- créer l’arborescence des unités d’organisation ;
- créer les groupes de sécurité ;
- créer plusieurs utilisateurs de test ;
- affecter automatiquement les utilisateurs aux groupes correspondants ;
- faciliter le déploiement initial de l’environnement Active Directory.

### Exemple de script

```powershell
Import-Module ActiveDirectory

$DomainDN = "DC=aegis,DC=local"
$BaseOU = "OU=AEGIS-ENTREPRISE,$DomainDN"

# Création de l'OU principale
New-ADOrganizationalUnit `
    -Name "AEGIS-ENTREPRISE" `
    -Path $DomainDN `
    -ProtectedFromAccidentalDeletion $true

# Création des sous-OU
$OUs = @(
    "Utilisateurs",
    "Groupes",
    "Ordinateurs",
    "Serveurs"
)

foreach ($OU in $OUs) {
    New-ADOrganizationalUnit `
        -Name $OU `
        -Path $BaseOU `
        -ProtectedFromAccidentalDeletion $true
}

# Création des groupes
$Groups = @(
    "Informatique",
    "RH",
    "Comptabilite"
)

foreach ($Group in $Groups) {
    New-ADGroup `
        -Name $Group `
        -GroupScope Global `
        -GroupCategory Security `
        -Path "OU=Groupes,$BaseOU"
}

# Demande du mot de passe utilisateur
$Password = Read-Host "Entrez le mot de passe temporaire des utilisateurs" -AsSecureString

# Création des utilisateurs
$Users = @(
    @{
        Prenom = "Jean"
        Nom = "Dupont"
        Login = "jdupont"
        Groupe = "Informatique"
    },
    @{
        Prenom = "Claire"
        Nom = "Martin"
        Login = "cmartin"
        Groupe = "RH"
    },
    @{
        Prenom = "Thomas"
        Nom = "Bernard"
        Login = "tbernard"
        Groupe = "Comptabilite"
    }
)

foreach ($User in $Users) {

    New-ADUser `
        -Name "$($User.Prenom) $($User.Nom)" `
        -GivenName $User.Prenom `
        -Surname $User.Nom `
        -SamAccountName $User.Login `
        -UserPrincipalName "$($User.Login)@aegis.local" `
        -Path "OU=Utilisateurs,$BaseOU" `
        -AccountPassword $Password `
        -Enabled $true `
        -ChangePasswordAtLogon $true

    Add-ADGroupMember `
        -Identity $User.Groupe `
        -Members $User.Login
}
```

Le mot de passe n’est pas stocké en clair dans le script. Il est demandé au moment de l’exécution avec `Read-Host -AsSecureString`.

---

## 🖥️ Intégration des postes Windows

Des postes clients Windows sont intégrés au domaine Active Directory afin de reproduire le fonctionnement d’un environnement d’entreprise.

Les postes clients permettent notamment de tester :

- l’attribution d’une configuration réseau ;
- la résolution DNS ;
- la communication avec le contrôleur de domaine ;
- l’intégration au domaine `aegis.local` ;
- l’authentification avec un compte Active Directory ;
- l’application des stratégies de groupe ;
- les droits d’accès des différents utilisateurs.

Les machines intégrées au domaine sont ensuite placées dans l’unité d’organisation dédiée aux ordinateurs.

---

## 🔐 Stratégies de groupe — GPO

Des stratégies de groupe sont progressivement mises en place afin de renforcer la sécurité et de standardiser la configuration des postes Windows.

Les GPO prévues ou mises en place concernent notamment :

- la politique de mots de passe ;
- le verrouillage des comptes après plusieurs tentatives échouées ;
- le verrouillage automatique des sessions ;
- la configuration du pare-feu Windows ;
- le renforcement de certains paramètres de sécurité ;
- la limitation de certains accès utilisateurs ;
- la gestion des paramètres Windows Defender ;
- le déploiement éventuel de ressources réseau.

Chaque stratégie sera testée depuis un poste client intégré au domaine.

La bonne application des GPO pourra notamment être vérifiée avec :

```powershell
gpupdate /force
```

Puis :

```powershell
gpresult /r
```

---

## 🧪 Tests & Validation

Chaque nouvelle fonctionnalité intégrée à Aegis Infra Lab fait l’objet de tests afin de vérifier son bon fonctionnement.

Les validations comprennent notamment :

- tests de résolution DNS ;
- attribution d’adresses IP via DHCP ;
- intégration d’un poste Windows au domaine ;
- authentification avec un compte du domaine ;
- application des GPO ;
- vérification des droits d’accès ;
- tests des règles de filtrage OPNsense ;
- vérification des communications entre les différentes zones réseau ;
- supervision des ressources système ;
- tests d’accès aux différents services ;
- tests de sauvegarde et de restauration.

Les captures d’écran et les résultats seront progressivement ajoutés à la documentation du projet.

---

## 📸 Documentation et preuves de fonctionnement

Le projet est documenté progressivement avec des captures d’écran et des résultats de tests.

Les éléments documentés pourront notamment inclure :

- structure Active Directory ;
- unités d’organisation ;
- utilisateurs et groupes ;
- intégration des postes au domaine ;
- GPO appliquées ;
- résultats de `gpresult` ;
- configuration DNS et DHCP ;
- règles OPNsense ;
- supervision Zabbix ;
- services Linux ;
- scripts PowerShell et Bash ;
- tests de sauvegarde et de restauration.

L’objectif est de pouvoir montrer non seulement la configuration mise en place, mais également son fonctionnement réel.

---

## 🚀 Évolutions prévues

Aegis Infra Lab est un projet évolutif.

Plusieurs améliorations pourront être ajoutées progressivement :

- intégration d’un SIEM ;
- centralisation des journaux Windows et Linux ;
- mise en place de scénarios de détection ;
- approfondissement de la supervision ;
- développement de nouvelles automatisations PowerShell et Bash ;
- conteneurisation de certains services ;
- amélioration de la stratégie de sauvegarde ;
- mise en place de tests de restauration plus complets ;
- exploration d’un environnement hybride avec des services cloud.

---
## 📁 Organisation du dépôt

Le dépôt est organisé afin de séparer la documentation, les scripts, les configurations, les captures d’écran et les tests réalisés.

```text
Aegis-Infra-Lab/
├── README.md
├── docs/
│   ├── architecture/
│   ├── installation/
│   ├── active-directory/
│   ├── network/
│   ├── linux/
│   └── security/
├── scripts/
│   ├── powershell/
│   └── bash/
├── configs/
├── screenshots/
│   ├── active-directory/
│   ├── windows-clients/
│   ├── gpo/
│   ├── dns-dhcp/
│   ├── opnsense/
│   ├── debian/
│   ├── nginx/
│   ├── zabbix/
│   └── backup/
└── tests/
```

Cette organisation évoluera progressivement avec l’avancement du laboratoire.

---

## 🐧 Environnement Linux — Debian 12

Une machine **Debian 12** est intégrée au laboratoire afin d’héberger différents services internes et de travailler sur l’administration Linux.

Cette machine permettra notamment de mettre en pratique :

- l’administration d’un serveur Linux ;
- la gestion des utilisateurs et des permissions ;
- la configuration réseau ;
- l’installation et la gestion de services ;
- la sécurisation du système ;
- l’utilisation de scripts Bash ;
- la supervision des ressources ;
- la consultation et l’analyse des journaux système.

La configuration sera progressivement documentée avec les commandes utilisées, les fichiers de configuration modifiés et les différents tests réalisés.

---

## 🌐 NGINX

NGINX sera utilisé comme service Web et reverse proxy au sein de la zone services.

Les objectifs sont notamment de travailler sur :

- l’installation et la configuration de NGINX ;
- l’hébergement de services Web internes ;
- la configuration d’un reverse proxy ;
- la gestion des virtual hosts ;
- la sécurisation des communications avec SSL/TLS ;
- la gestion des ports et des règles réseau ;
- la journalisation des accès et des erreurs.

Des tests seront réalisés afin de vérifier l’accès aux services depuis les réseaux autorisés.

---

## 📊 Supervision avec Zabbix

Zabbix sera utilisé afin de superviser progressivement les différents équipements et serveurs du laboratoire.

La supervision pourra notamment concerner :

- Windows Server 2022 ;
- les postes Windows ;
- Debian 12 ;
- certains services réseau ;
- l’utilisation du processeur ;
- la mémoire ;
- l’espace disque ;
- la disponibilité des machines ;
- l’état des services ;
- certains événements système.

Des alertes pourront également être configurées afin de détecter les indisponibilités ou certains comportements anormaux.

La partie supervision sera documentée avec :

- l’ajout des hôtes ;
- la configuration des agents ;
- les métriques collectées ;
- les tableaux de bord ;
- les alertes ;
- les tests de disponibilité.

---

## 💾 Sauvegarde & Restauration

Une stratégie de sauvegarde sera progressivement mise en place afin de travailler sur la protection des données et la continuité de service.

Les objectifs sont notamment de :

- sauvegarder certaines configurations importantes ;
- sauvegarder les données nécessaires au laboratoire ;
- conserver plusieurs copies ;
- séparer les sauvegardes du reste de l’infrastructure ;
- documenter les procédures de sauvegarde ;
- effectuer des tests de restauration.

Une approche inspirée de la règle **3-2-1** sera appliquée dans la mesure du possible au sein du laboratoire.

Les tests permettront notamment de vérifier :

- le bon déroulement des sauvegardes ;
- l’intégrité des données ;
- la disponibilité des fichiers ;
- la restauration effective des données ;
- le temps nécessaire à une restauration.

---

## 🔄 Automatisation Linux avec Bash

En complément de PowerShell pour l’environnement Windows, Bash sera utilisé afin d’automatiser certaines tâches Linux.

Les scripts pourront notamment permettre de :

- automatiser certaines installations ;
- récupérer des informations système ;
- vérifier l’état des services ;
- automatiser certaines tâches d’administration ;
- effectuer des contrôles de disponibilité ;
- faciliter la maintenance de Debian.

Les scripts seront progressivement ajoutés au dépôt avec leur documentation.

---

## 🔎 Journalisation

La journalisation fait partie du projet afin de mieux comprendre le fonctionnement des différents systèmes et services.

Les journaux pourront notamment être utilisés pour analyser :

- les connexions utilisateurs ;
- les événements Windows ;
- les événements Active Directory ;
- les logs OPNsense ;
- les journaux Linux ;
- les logs NGINX ;
- les événements Zabbix ;
- les erreurs système ;
- les tentatives de connexion.

À terme, une centralisation des journaux pourra être mise en place afin de préparer l’intégration d’une solution SIEM.

---

## 🛡️ Sécurisation Linux

La machine Debian sera progressivement durcie afin de limiter sa surface d’attaque.

Les mesures pourront notamment comprendre :

- mise à jour régulière du système ;
- suppression ou désactivation des services inutiles ;
- gestion stricte des utilisateurs et des permissions ;
- sécurisation des accès distants ;
- limitation des ports exposés ;
- contrôle des services actifs ;
- surveillance des journaux ;
- sécurisation de NGINX ;
- utilisation de SSL/TLS lorsque nécessaire.

Chaque modification importante sera testée afin de vérifier qu’elle n’empêche pas le fonctionnement normal des services.

---

## 📸 Documentation & Captures

Les différentes étapes d’Aegis Infra Lab sont documentées avec des captures d’écran afin de montrer le fonctionnement réel de l’infrastructure et les résultats obtenus.

Les captures sont classées par thème dans le dossier :

```text
screenshots/
├── active-directory/
├── windows-clients/
├── gpo/
├── dns-dhcp/
├── opnsense/
├── debian/
├── nginx/
├── zabbix/
└── backup/
```

### 🗂️ Active Directory

Captures prévues :

- structure des unités d’organisation ;
- utilisateurs créés ;
- groupes de sécurité ;
- appartenance des utilisateurs aux groupes.

Exemple :

```markdown
![Structure Active Directory](screenshots/active-directory/ad-structure.png)
```

---

### 🖥️ Postes Windows

Captures prévues :

- poste Windows intégré au domaine `aegis.local` ;
- machine visible dans Active Directory ;
- ouverture de session avec un compte du domaine ;
- configuration réseau du poste.

Exemple :

```markdown
![Poste intégré au domaine](screenshots/windows-clients/domain-join.png)
```

---

### 🔐 GPO

Captures prévues :

- stratégies de groupe créées ;
- liaison des GPO aux unités d’organisation ;
- résultat de `gpupdate /force` ;
- résultat de `gpresult /r` ;
- preuve qu’une stratégie est réellement appliquée sur le poste client.

Exemple :

```markdown
![GPO appliquées](screenshots/gpo/gpresult.png)
```

---

### 🌐 DNS & DHCP

Captures prévues :

- zone DNS du domaine ;
- enregistrements DNS ;
- étendue DHCP ;
- bail DHCP attribué à un poste client ;
- résultats de `nslookup` ;
- résultats de `ipconfig /all`.

Exemple :

```markdown
![Configuration DHCP](screenshots/dns-dhcp/dhcp-scope.png)
```

---

### 🔥 OPNsense

Captures prévues :

- interfaces réseau ;
- règles de pare-feu ;
- segmentation des différentes zones ;
- test de communication autorisée ;
- test de communication bloquée.

Exemple :

```markdown
![Règles OPNsense](screenshots/opnsense/firewall-rules.png)
```

---

### 🐧 Debian 12

Captures prévues :

- configuration réseau ;
- services actifs ;
- utilisateurs et permissions ;
- état du système ;
- tests de communication avec les autres machines.

Exemple :

```markdown
![Serveur Debian](screenshots/debian/debian-network.png)
```

---

### 🌍 NGINX

Captures prévues :

- installation du service ;
- configuration NGINX ;
- service actif ;
- page Web accessible ;
- reverse proxy ;
- configuration SSL/TLS.

Exemple :

```markdown
![NGINX](screenshots/nginx/nginx-service.png)
```

---

### 📊 Zabbix

Captures prévues :

- tableau de bord ;
- hôtes supervisés ;
- métriques Windows et Linux ;
- disponibilité des machines ;
- alertes configurées.

Exemple :

```markdown
![Dashboard Zabbix](screenshots/zabbix/dashboard.png)
```

---

### 💾 Sauvegarde & Restauration

Captures prévues :

- configuration de la sauvegarde ;
- exécution d’une sauvegarde ;
- résultat du job ;
- restauration d’un fichier ou d’une configuration ;
- preuve du succès de la restauration.

Exemple :

```markdown
![Test de restauration](screenshots/backup/restore-test.png)
```

---

## ✅ Principe de validation

Pour chaque technologie mise en place, l’objectif est de conserver au minimum :

1. une capture de la configuration ;
2. une capture du test réalisé ;
3. une capture du résultat obtenu.

Cela permet de montrer non seulement que la technologie a été installée, mais également qu’elle fonctionne réellement dans le laboratoire.

---

## 📌 État du projet

🚧 **Aegis Infra Lab est actuellement en cours de développement.**

### ✅ Déjà réalisé

- création de l’environnement virtualisé ;
- déploiement d’OPNsense ;
- mise en place de la segmentation réseau ;
- installation de Windows Server 2022 ;
- déploiement d’Active Directory Domain Services ;
- création du domaine `aegis.local` ;
- création de la structure des unités d’organisation ;
- création des groupes de sécurité ;
- création des comptes utilisateurs de test ;
- mise en place des services DNS et DHCP ;
- automatisation d’une partie de la configuration Active Directory avec PowerShell.

### 🔄 En cours

- intégration des postes Windows au domaine ;
- authentification avec les comptes Active Directory ;
- mise en place des stratégies de groupe ;
- tests des GPO ;
- documentation des différentes étapes ;
- ajout des captures de validation.

### ⏳ Prochaines étapes

- finalisation des règles de filtrage OPNsense ;
- déploiement de Debian 12 ;
- configuration de NGINX ;
- déploiement de Zabbix ;
- mise en place de la supervision ;
- mise en place de la stratégie de sauvegarde ;
- tests de restauration ;
- développement de scripts Bash ;
- approfondissement de la journalisation ;
- amélioration du durcissement des systèmes.

---

## 🚀 Évolutions prévues

Une fois l’infrastructure principale stabilisée, plusieurs évolutions pourront être ajoutées :

- intégration d’un SIEM ;
- centralisation des logs Windows et Linux ;
- création de règles de détection ;
- scénarios de détection d’incidents ;
- automatisation plus avancée ;
- utilisation de Docker pour certains services ;
- ajout de nouvelles machines Linux ;
- amélioration de la supervision ;
- tests de restauration plus avancés ;
- exploration d’un environnement cloud ou hybride.

---

## 🎯 Finalité du projet

Aegis Infra Lab a pour objectif de reproduire progressivement une infrastructure informatique d’entreprise cohérente, segmentée et sécurisée.

Ce laboratoire me permet de mettre en pratique mes connaissances en :

- administration Windows et Linux ;
- Active Directory ;
- DNS et DHCP ;
- gestion des utilisateurs, groupes et droits d’accès ;
- stratégies de groupe ;
- réseau et segmentation ;
- pare-feu et filtrage ;
- supervision ;
- sauvegarde et restauration ;
- automatisation ;
- journalisation ;
- sécurisation des infrastructures.

L’objectif est également de disposer d’un projet concret permettant de présenter les configurations réalisées, les choix techniques, les scripts développés et les différents tests de validation.

---

## 🔗 Liens

- **LinkedIn :** à compléter
- **GitHub :** https://github.com/kieferalexandre1-creator

---

### 🛡️ Aegis Infra Lab

**Projet personnel — Systèmes, Réseaux & Cybersécurité**

Construit, testé et documenté progressivement.
