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

---

### 📜 Code source du script

```powershell
# ==============================================================================
# Nom du script : Deploy-AegisAD.ps1
# Description   : Automatisation du déploiement AD pour l'infrastructure Aegis
# Domaine       : aegis.local
# ==============================================================================

# 1. Structure des Unités d'Organisation (OU)
$ouBase = "OU=AEGIS-ENTREPRISE,DC=aegis,DC=local"

New-ADOrganizationalUnit -Name "AEGIS-ENTREPRISE" -Path "DC=aegis,DC=local" -ErrorAction SilentlyContinue
New-ADOrganizationalUnit -Name "Utilisateurs" -Path $ouBase -ErrorAction SilentlyContinue
New-ADOrganizationalUnit -Name "Groupes" -Path $ouBase -ErrorAction SilentlyContinue
New-ADOrganizationalUnit -Name "Ordinateurs" -Path $ouBase -ErrorAction SilentlyContinue
New-ADOrganizationalUnit -Name "Serveurs" -Path $ouBase -ErrorAction SilentlyContinue

# 2. Création des Groupes de sécurité par service
$ouGroupes = "OU=Groupes,$ouBase"
$groupes = @("GRP_Informatique", "GRP_Ressources-Humaines", "GRP_Comptabilite")

foreach ($g in $groupes) {
    New-ADGroup -Name $g -GroupScope Global -GroupCategory Security -Path $ouGroupes -ErrorAction SilentlyContinue
}

# 3. Création des Utilisateurs et affectation aux groupes
$ouUsers = "OU=Utilisateurs,$ouBase"
$users = @(
    @{Prenom="Jean"; Nom="Dupont"; Service="Informatique"},
    @{Prenom="Claire"; Nom="Martin"; Service="Ressources-Humaines"},
    @{Prenom="Thomas"; Nom="Bernard"; Service="Comptabilite"}
)

foreach ($u in $users) {
    $sam = ($u.Prenom.Substring(0,1) + $u.Nom).ToLower()
    $upn = "$sam@aegis.local"
    $grp = "GRP_" + $u.Service

    New-ADUser -Name "$($u.Prenom) $($u.Nom)" `
               -GivenName $u.Prenom `
               -Surname $u.Nom `
               -SamAccountName $sam `
               -UserPrincipalName $upn `
               -Path $ouUsers `
               -Enabled $true `
               -AccountPassword (ConvertTo-SecureString "P@ssword2026!" -AsPlainText -Force) `
               -ChangePasswordAtLogon $true `
               -ErrorAction SilentlyContinue

    Add-ADGroupMember -Identity $grp -Members$sam -ErrorAction SilentlyContinue
}



