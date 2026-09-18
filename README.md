# Aegis-Infra-Lab - Infrastructure d'Entreprise Sécurisée 
### 👤 Alexandre KIEFER
**Administrateur Systèmes, Réseaux & Cybersécurité**  
📍 Savigny-sur-Orge, Île-de-France  
🔗 [LinkedIn](https://www.linkedin.com/in/alexandre-kiefer-847334282/) | 🐙 [GitHub](https://github.com/kieferalexandre1-creator) | ✉️ kiefer.alexandre1@gmail.com

[![Statut](https://img.shields.io/badge/Statut-En%20d%C3%A9veloppement-orange)](#)
[![OS](https://img.shields.io/badge/Environnement-VirtualBox-blue)](#)
# 🎯 Projet Professionnel & Recherche d'Emploi

## 👤 À propos
Titulaire d'un **Bachelor Administrateur d’Infrastructures Sécurisées** (avec une solide expérience sur le terrain en alternance et en support IT), je suis actuellement à la recherche d'un **CDI**.

## 💼 Postes visés
* **Administrateur / Technicien Système & Réseau**
* **Technicien Support N1 / N2 / N3**
* **Gestionnaire d'Infrastructures & Sécurité IT**

## 💡 Ma Démarche & Ce Projet (`Aegis-Infra-Lab`)
Afin de maintenir une pratique constante et de faire évoluer mes compétences, j'ai conçu ce laboratoire d'infrastructure virtualisé. Il illustre ma capacité à :
* **Déployer et administrer des annuaires d'entreprise** (Active Directory, automatisation PowerShell, gestion RBAC).
* **Segmenter et sécuriser les réseaux** (Pare-feu OPNsense/pfSense, routage, VLANs).
* **Industrialiser et documenter** (Scripts d'installation, suivi rigoureux sous Git).

---

## 📜 Certifications IT prioritaires pour les profils Juniors

Pour valider et renforcer mes compétences terrain, voici les certifications adaptées aux postes d'administrateur et de support avancé :

### 1. Système & Cloud (Microsoft)
* **Microsoft Certified: Windows Server Hybrid Administrator Associate (AZ-800 & AZ-801)** : La référence idéale pour valider l'administration Active Directory, Hyper-V, le stockage et l'interconnexion hybride Azure.
* **Microsoft Certified: Azure Fundamentals (AZ-900)** : Certification d'entrée pour valider la compréhension globale des services cloud Microsoft.

### 2. Réseau & Sécurité Périmétrique
* **Cisco CCNA (200-301)** : Le standard incontournable pour prouver la maîtrise des fondamentaux réseaux (routage, commutation, IPv4/IPv6, VLANs, sécurité de base).
* **CompTIA Network+** : Une alternative neutre vis-à-vis des constructeurs pour valider la gestion des réseaux d'entreprise.

### 3. Sécurité & Bonnes Pratiques
* **CompTIA Security+ (SY0-701)** : La certification sécurité la plus demandée par les recruteurs pour les profils juniors. Elle couvre les concepts clés du durcissement, de la gestion des vulnérabilités et des accès.

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
