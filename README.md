# Aegis-Infra-Lab - Infrastructure d'Entreprise Sécurisée 
### 👤 Alexandre KIEFER
**Administrateur Systèmes, Réseaux & Cybersécurité**  
📍 Savigny-sur-Orge, Île-de-France  
🔗 [LinkedIn](https://www.linkedin.com/in/alexandre-kiefer-847334282/) | 🐙 [GitHub](https://github.com/kieferalexandre1-creator) | ✉️ kiefer.alexandre1@gmail.com

[![Statut](https://img.shields.io/badge/Statut-En%20d%C3%A9veloppement-orange)](#)
[![OS](https://img.shields.io/badge/Environnement-VirtualBox-blue)

# 🎯 Projet Professionnel & Recherche d'Emploi

## 👤 À propos
Diplômé d'un **BTS Technicien Informatique** et d'un **Bachelor Administrateur d’Infrastructures Sécurisées**, je cumule **1 an d'alternance** en administration système, réseau et cybersécurité, complété par un **stage de 3 mois** en tant que technicien informatique. Fort de cette expérience de terrain, je suis actuellement à la recherche d'un poste en **CDI**.

## 💼 Postes visés
* **Technicien Informatique / Support IT (N1, N2, N3)**
* **Technicien / Administrateur Système & Réseau**
* **Gestionnaire / Technicien d'Infrastructures**
* **Technicien / Analyste Sécurité Informatique (SOC)**
* **Consultant / Technicien Déploiement & Migration**

## 💡 Ma Démarche & Ce Projet (`Aegis-Infra-Lab`)
Afin de maintenir une pratique constante et de valoriser mes compétences, j'ai conçu ce laboratoire d'infrastructure virtualisé. Il illustre ma capacité à :
* **Gérer le support et l'annuaire d'entreprise** (Active Directory, automatisation PowerShell, gestion RBAC, dépannage).
* **Segmenter et sécuriser les réseaux** (Pare-feu OPNsense/pfSense, routage, VLANs).
* **Industrialiser, superviser et documenter** (Scripts de déploiement, suivi sous Git).

---

## 📜 Certifications IT prioritaires pour mon profil

Pour valider officiellement mes compétences terrain :

### 1. Support & Fondamentaux
* **CompTIA A+** : Référence internationale pour le support, le dépannage matériel/système et la relation utilisateur.
* **Microsoft Certified: Azure Fundamentals (AZ-900)** : Validation de la compréhension des environnements cloud hybrides.

### 2. Administration Système & Réseau
* **Microsoft Certified: Windows Server Hybrid Administrator Associate (AZ-800 / AZ-801)** : La certification clé pour valider la maîtrise d'Active Directory, Hyper-V et Windows Server.
* **Cisco CCNA (200-301)** ou **CompTIA Network+** : Incontournable pour prouver la maîtrise du réseau (VLANs, routage, commutation).

### 3. Sécurité
* **CompTIA Security+ (SY0-701)** : La certification de référence pour valoriser la gestion des accès, le durcissement d'infrastructure et les bonnes pratiques de sécurité.
  
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
  
## Deploy-AegisAD.ps1
Voici le bloc Markdown complet à intégrer dans le README.md de ton projet GitHub, avec la section Code source intégrée et formatée pour mettre en valeur ton script.

Markdown
## 🛠️ Automatisation Active Directory (`Deploy-AegisAD.ps1`)

Le déploiement de l'arborescence, des groupes de sécurité et des utilisateurs du domaine `aegis.local` est entièrement automatisé via le script PowerShell `Deploy-AegisAD.ps1`.

### 📌 Fonctionnalités du script
* **Structure d'OU** : Création de l'OU racine `AEGIS-ENTREPRISE` et des sous-OU (`Utilisateurs`, `Groupes`, `Ordinateurs`, `Serveurs`).
* **Groupes de sécurité** : Création des groupes globaux par service (`GRP_Informatique`, `GRP_Ressources-Humaines`, `GRP_Comptabilite`).
* **Provisioning Utilisateurs** : Création des comptes avec identifiants normalisés (`jdupont`, `cmartin`, `tbernard`), mot de passe temporaire et réinitialisation obligatoire à la première connexion.
* **Gestion des membres** : Affectation automatique de chaque utilisateur à son groupe respectif.

### Code source du script

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

Exécution
Pour exécuter le script sur le Contrôleur de Domaine (SRV-AD001), ouvrir PowerShell en tant qu'administrateur :
