# CodéConneries

Ce projet est un réseau social en PHP sur le thème du développement informatique dont les objectifs généraux sont : 
- faire un site web dynamique qui construit les pages HTML à la demande grâce à une base de données,
- enrichir ce site de nouveaux contenus fournis par les utilisateurs avec des formulaires,
- gérer les authentifications (login), sessions, autorisations (droits d’accès) et inscriptions,
- avoir un premier aperçu de la conception web, de la conception de base de données, des problématiques d’un projet multi-langages.

## Equipe de 4 personnes

Jérémie PATOT - Gilbert MOUGAMADOU - Bastien VINTRAS - Ghislaine AYBRAM

## Demo

Insert gif or link to demo

## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)

## Tech Stack

**Langages:** PHP, SQL, HTML, CSS
**Database:** MySQL

# Fonctionnalités ajoutées
- [x] refactoring du code existant,
- [x] ajout partout où un utilisateur (auteur, contact, etc) est mentionné d'un lien qui mène vers le mur de cet utilisateur,
- [x] ajout d'une page d'inscription au réseau social,
- [x] ajout d'une page de connexion (avec notions de session),
- [x] ajout d'un formulaire d’ajout de message quand l'utilisateur est connecté (publication sur son propre mur),
- [x] ajout d'un formulaire d’abonnement les murs des autres utilisateurs,
- [x] ajout d'un formulaire pour gérer les likes sur les messages,
- [x] interdictions des pages feed, settings, followers et subscriptions tant que la connexion n’a pas été validée,
- [x] changement du menu profil pour qu’il pointe vers la page de connexion quand l'utilisateur n'est pas connecté,
- [x] séparer les messages en paragraphes (mettre les paragraphes entre balise <p>),
- [x] analyse des #tags (1/2) : lors de la soumission d’un message analyse du texte pour repérer les mots commençant par un dièse "#" et si besoin ajout du mot-clé inconnu dans la table tags,
- [x] utilisation d'une bibliothèque CSS (Bootstrap)

# Reste à implémenter
- [ ] analyse des #tags (2/2) : ajout dans la table posts_tags du lien entre le post et le tag,
- [ ] ajout partout où un mot-clé est mentionné un lien vers la page du mot clé correspondant,
- [ ] permettre à l’utilisateur de “répondre” à un message (à l'aide du champs “parent_id” dans la table “posts” pour noter à quel message correspond cette réponse),
- [ ] permettre le chargement de nouveaux commentaires quand on arrive en fin de page (sans recharger la page) via une bibliothèque javascript comme jquery,
