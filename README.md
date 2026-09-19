# Aegis-Infra-Lab - Infrastructure d'Entreprise Sécurisée 
### 👤 Alexandre KIEFER
**Administrateur Systèmes, Réseaux & Cybersécurité**  
📍 Savigny-sur-Orge, Île-de-France  
🔗 [LinkedIn](https://www.linkedin.com/in/alexandre-kiefer-847334282/) | 🐙 [GitHub](https://github.com/kieferalexandre1-creator) | ✉️ kiefer.alexandre1@gmail.com

[![Statut](https://img.shields.io/badge/Statut-En%20d%C3%A9veloppement-orange)](#)
[![OS](https://img.shields.io/badge/Environnement-VirtualBox-blue)

## 👤 À propos de moi

Profil **junior en administration systèmes, réseaux et cybersécurité**, titulaire d’un **Titre Professionnel Technicien Informatique obtenu en 2024** et d’un **Bachelor Administrateur d’Infrastructures Sécurisées obtenu en 2025**.

Mon parcours m’a permis d’acquérir une première expérience professionnelle de **3 mois en tant que Technicien Informatique**, puis d’environ **1 an en alternance en tant qu’Administrateur Systèmes, Réseaux & Cybersécurité**.

J’ai notamment eu l’occasion de travailler sur des environnements Windows et Linux, la virtualisation avec VMware ESXi/vCenter, les réseaux, la sauvegarde, la supervision, la gestion des comptes et des droits d’accès ainsi que la sécurisation des infrastructures.

Je souhaite aujourd’hui continuer à développer mes compétences et poursuivre mon parcours avec un **Mastère Expert Cybersécurité en alternance**.

Aegis Infra Lab me permet de mettre en pratique mes connaissances dans un environnement personnel, de tester différentes technologies et de documenter progressivement mon travail.

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

```text
Aegis-Infra-Lab/
├── README.md
├── docs/
│   ├── architecture/
│   ├── installation/
│   └── security/
├── scripts/
│   ├── powershell/
│   └── bash/
├── configs/
└── screenshots/
```

---

## 📌 État du projet

🚧 **Projet actuellement en cours de développement**

Les différentes briques de l’infrastructure sont mises en place progressivement puis testées et documentées.

### Étapes en cours

- finalisation de l’environnement Active Directory ;
- intégration des postes Windows au domaine ;
- mise en place des GPO ;
- tests des comptes utilisateurs et des droits d’accès ;
- ajout progressif des captures et preuves de fonctionnement.

### Étapes suivantes

- finalisation de la zone services Linux ;
- mise en place de NGINX ;
- déploiement de Zabbix ;
- amélioration des règles de filtrage réseau ;
- mise en place de la stratégie de sauvegarde ;
- automatisation de nouvelles tâches avec PowerShell et Bash.

---

## 🎯 Objectif final

L’objectif d’Aegis Infra Lab est de construire progressivement une infrastructure d’entreprise sécurisée dans un environnement virtualisé.

Ce laboratoire me permet de mettre en pratique et de documenter mes compétences en :

- administration Windows et Linux ;
- Active Directory ;
- DNS et DHCP ;
- gestion des utilisateurs et des groupes ;
- GPO ;
- segmentation réseau ;
- filtrage avec OPNsense ;
- supervision ;
- sauvegarde ;
- automatisation ;
- sécurisation des infrastructures.

Le projet continuera d’évoluer au fur et à mesure de ma progression et de l’intégration de nouvelles technologies.