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
![WordPress](path/to/wordpress-screenshot.png)

#### Grafana
![Grafana](path/to/grafana-screenshot.png)

#### Prometheus
![Prometheus](path/to/prometheus-screenshot.png)

#### cAdvisor
![cAdvisor](path/to/cadvisor-screenshot.png)

## Installation

Pour installer ce projet localement, suivez les étapes ci-dessous :

1. Clonez le dépôt sur votre machine :
   ```bash
   git clone https://github.com/votre-utilisateur/tp-groupe-5-hamara.git
   
2. Naviguez dans le répertoire du projet :
  ```bash
   cd Tp_Docker_Swarm_Groupe5_Hamara

3. Initialisez le cluster Docker Swarm :
  ```bash
   docker swarm init


