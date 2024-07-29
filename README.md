# Tp groupe 5 (hamara)

## Table des matières

1. [Introduction](#introduction)
2. [Projet Réalisé](#projet-réalisé)
3. [Installation](#installation)
4. [Utilisation](#utilisation)
5. [Contributeurs](#contributeurs)
6. [Licence](#licence)

## Introduction

Bienvenue dans le projet "Tp groupe 5 (hamara)". Ce projet a été réalisé dans le cadre de notre cours sur les conteneurs et DevOps. L'objectif de ce projet est de mettre en place un cluster Docker utilisant Docker Swarm, avec le déploiement de plusieurs applications pour démontrer la haute disponibilité, la supervision et le monitoring, ainsi que la sauvegarde et la réplication des données.

## Projet Réalisé

### Objectifs

Le projet a pour but de :

- Créer un cluster Docker Swarm.
- Déployer une application WordPress.
- Déployer des applications de supervision et de monitoring (Grafana, Prometheus, cAdvisor).
- Mettre en place GlusterFS pour la sauvegarde et la réplication des données.
- Utiliser Keepalived pour assurer la haute disponibilité (HA) du cluster.
- Configurer des alertes sur Discord pour les états critiques des nœuds.

### Technologies Utilisées

- **Docker Swarm** : Pour la gestion du cluster Docker.
- **WordPress** : Pour déployer une application web de gestion de contenu.
- **Grafana, Prometheus, cAdvisor** : Pour la supervision et le monitoring.
- **GlusterFS** : Pour la sauvegarde et la réplication des données.
- **Keepalived** : Pour assurer la haute disponibilité du cluster.
- **Discord** : Pour les alertes sur les états critiques des nœuds.

### Architecture

1. **Cluster Docker Swarm** :
    - Un cluster de plusieurs nœuds Docker pour assurer la répartition de la charge et la redondance.
    
2. **Stack 1 - WordPress** :
    - Déploiement de WordPress avec une base de données MySQL.

3. **Stack 2 - Supervision et Monitoring** :
    - Déploiement de Grafana pour la visualisation.
    - Déploiement de Prometheus pour la collecte des métriques.
    - Déploiement de cAdvisor pour la surveillance des conteneurs.

4. **GlusterFS** :
    - Implémentation de GlusterFS pour la sauvegarde et la réplication des données sur différents nœuds du cluster.

5. **Keepalived** :
    - Configuration de Keepalived pour la gestion de l'adresse IP virtuelle, garantissant la haute disponibilité.

6. **Alertes Discord** :
    - Configuration des alertes pour remonter les différents états critiques des nœuds via Discord.

### Captures d'Écran

#### WordPress
![WordPress]

<img width="956" alt="image" src="https://github.com/user-attachments/assets/ce618acf-a879-4d7e-9ae7-c5cfbdc79979">

<img width="958" alt="image" src="https://github.com/user-attachments/assets/aa3d0c39-5108-4d85-ae6b-70966fc9c872">

<img width="959" alt="image" src="https://github.com/user-attachments/assets/b07d624e-0632-4565-82cc-36387f3d1522">



#### Grafana
![Grafana]

<img width="941" alt="Grafana" src="https://github.com/user-attachments/assets/73140f85-5759-4d81-a9bf-66305455c591">


#### Prometheus
![Prometheus]

<img width="890" alt="Prometheus" src="https://github.com/user-attachments/assets/5a3f2dc6-6579-4e46-a010-ea3311181937">

##Alertes

<img width="689" alt="image" src="https://github.com/user-attachments/assets/6fc1f67c-2210-4392-929a-69c28f707a59">

<img width="805" alt="image" src="https://github.com/user-attachments/assets/fda5b7ea-2b83-4baf-a574-9b5f02001a1d">


#### cAdvisor
![cAdvisor]

<img width="942" alt="image" src="https://github.com/user-attachments/assets/ed627d68-a535-4c89-80bb-20fe4cff1dc2">


## Installation

Pour installer ce projet localement, suivez les étapes ci-dessous :

1. Clonez le dépôt sur votre machine :
   ```bash
   git clone https://github.com/votre-utilisateur/tp-groupe-5-hamara.git
   
2. Naviguez dans le répertoire du projet :
  ```bash
   cd Tp_Docker_Swarm_Groupe5_Hamara
  ```


3. Initialisez le cluster Docker Swarm :
  ```bash
   docker swarm init
  ```


