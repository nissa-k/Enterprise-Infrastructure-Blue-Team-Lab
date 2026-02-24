# Enterprise-Infrastructure-Blue-Team-Lab
Overview

Ce repository documente la mise en place d’une infrastructure complète orientée détection, supervision et sécurisation d’un système d’information.

L’objectif est de reproduire une architecture d’entreprise réaliste intégrant :

Services d’infrastructure (DHCP, DNS, NTP, Active Directory)

Serveurs Linux et Windows

Segmentation réseau

Supervision et centralisation des logs

Durcissement système

Contrôle des accès et politiques de sécurité

Ce laboratoire s’inscrit dans une démarche Blue Team : prévention, détection, analyse et réponse aux incidents.

Architecture
Environnement

Infrastructure déployée en environnement virtualisé :

VirtualBox / VMware

Réseaux segmentés (LAN, DMZ, réseau d’administration)

Pare-feu dédié (pfSense)

Contrôleur de domaine Windows

Serveurs Linux (services applicatifs)

Serveur de supervision centralisé

Objectif : simuler un système d’information d’entreprise avec contrôle des flux et journalisation centralisée.

Infrastructure Core Services
DHCP Server

Attribution dynamique des adresses IP

Configuration des passerelles et DNS

Gestion des plages d’adressage

Analyse des baux

Impact sécurité

Contrôle des équipements autorisés

Surveillance des connexions réseau

DNS Server

Zones internes

Résolution locale sécurisée

Intégration avec Active Directory

Diagnostic via dig / nslookup

Impact sécurité

Prévention des résolutions non autorisées

Cohérence des services internes

NTP Server

Synchronisation centralisée

Configuration chrony / ntpd

Importance Blue Team

Corrélation fiable des logs

Intégrité temporelle pour investigation

Windows Server & Identity Management
Active Directory

Déploiement d’un contrôleur de domaine

Création d’OU

Gestion des utilisateurs et groupes

GPO (stratégies de sécurité)

Politique de mot de passe renforcée

Permissions NTFS et partages sécurisés

Approche sécurité

Principe du moindre privilège

Séparation des rôles

Restriction des accès administratifs

Journalisation des événements AD

Linux Servers Hardening
Services installés

SSH sécurisé (authentification par clé, désactivation root)

Apache / Nginx

PHP

MySQL

FTP configuré avec isolation

Mesures de durcissement

Configuration firewall (UFW / iptables)

Restriction des ports exposés

Permissions strictes

Surveillance des logs système

Mise à jour régulière des paquets

Network Security
pfSense Firewall
Configuration

NAT

Règles firewall granulaires

Segmentation réseau

VPN IPsec

WireGuard

Objectif Blue Team

Contrôle des flux inter-segments

Réduction de la surface d’attaque

Isolation des services critiques

Journalisation des connexions

Monitoring & Log Management
Wazuh (SIEM / HIDS)

Déploiement d’agents

Surveillance d’intégrité des fichiers

Détection d’anomalies

Alertes sur événements critiques

Graylog

Centralisation des logs

Corrélation d’événements

Analyse en temps réel

Création de dashboards

Compétences développées

Lecture et interprétation de logs

Détection d’activités suspectes

Analyse post-incident

Corrélation multi-sources

Network Analysis & Threat Detection
Outils utilisés

Nmap

Wireshark

tcpdump

Scan de services

Analyse TCP / UDP / DNS

Approche Blue Team

Identification des services exposés

Détection d’anomalies réseau

Surveillance du trafic interne

Cryptography & Secure Communications
Implémentation

TLS

Certificats

Hash SHA-256 / SHA-512

GPG (chiffrement & signature)

IPsec

Objectif

Protection des données en transit

Vérification d’intégrité

Sécurisation des communications internes

Virtualization & Containerization
Virtualisation

VirtualBox / VMware

Création d’environnements isolés

Conteneurisation

Docker

Docker Compose

Conteneurisation de services

Objectif sécurité

Isolation des applications

Reproductibilité des environnements

Tests d’attaque en laboratoire contrôlé

Blue Team Skills Developed

Administration Windows Server & Active Directory

Durcissement Linux

Segmentation réseau

Configuration firewall avancée

Gestion des identités et des accès

Centralisation et analyse de logs

Détection d’événements de sécurité

Compréhension des techniques d’attaque courantes

Investigation post-incident

Security Mindset

Ce laboratoire est conçu avec une approche défensive :

Principe du moindre privilège

Réduction de la surface d’exposition

Journalisation systématique

Segmentation réseau

Surveillance continue

Tous les tests ont été réalisés en environnement isolé.
