# Azure Application Gateway Lab

## Objectif

Déployer une infrastructure web hautement disponible sur Microsoft Azure en utilisant Azure Application Gateway pour distribuer le trafic vers plusieurs serveurs web.

---

## Technologies utilisées

- Microsoft Azure
- Azure Application Gateway
- Windows Server
- IIS
- Virtual Network (VNet)
- Network Security Groups (NSG)

---

## Architecture

Internet
    │
    ▼
Application Gateway
    │
    ▼
Backend Pool
 ├── VM1 (IIS)
 └── VM2 (IIS)

---

## Étapes réalisées

### 1. Création du réseau

- Création d'un Virtual Network
- Création des sous-réseaux :
  - appgw-subnet
  - backend-subnet

### 2. Déploiement des serveurs

- Création de deux machines virtuelles Windows Server
- Installation du rôle IIS
- Configuration d'une page web différente sur chaque serveur

### 3. Configuration de l'Application Gateway

- Création du Backend Pool
- Configuration du Health Probe
- Création du Listener HTTP
- Création des règles de routage

### 4. Validation

- Vérification de l'état Healthy des serveurs
- Test d'accès via l'adresse IP publique de l'Application Gateway

---

## Captures d'écran

À venir

---

## Compétences démontrées

- Administration Azure
- Réseau Cloud
- Haute disponibilité
- Répartition de charge
- Dépannage réseau
- Administration Windows Server
- IIS

---

## Auteur

Jair Da Silva

Support IT N1/N2 | Technicien Systèmes & Réseaux | Cloud Azure
