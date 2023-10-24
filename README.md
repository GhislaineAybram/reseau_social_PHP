# CodéConneries - réseau social sur le thème du développement informatique

Ce projet est un réseau social en PHP sur le thème du développement informatique dont les objectifs généraux sont : 
- travailler sur un code pré-éxistant (ce qui correspond à une réalité professionnelle fréquente),
- faire un site web dynamique qui construit les pages HTML à la demande grâce à une base de données,
- enrichir ce site de nouveaux contenus fournis par les utilisateurs avec des formulaires,
- gérer les authentifications (login), sessions, autorisations (droits d’accès) et inscriptions,
- avoir un premier aperçu de la conception web, de la conception de base de données, des problématiques d’un projet multi-langages.

## Equipe de 4 personnes - 6 jours

Jérémie PATOT - Gilbert MOUGAMADOU - Bastien VINTRAS - Ghislaine AYBRAM

## Aperçu du projet

*La page actualités du réseau social*
![App Screenshot](/screen/res_soc_actualites.jpg)

*Le mur de l'utilisateur connecté qui présente ses messages*
![App Screenshot](/screen/res_soc_mur_utilisateur.jpg)

*La page de présentation des mots clefs avec système d'abonnement aux mots clefs*
![App Screenshot](/screen/res_soc_mots_clefs.jpg)

*Les personnes auxquelles l'utilisateur s'est abonné*
![App Screenshot](/screen/res_soc_abonnements.jpg)

## Tech Stack

- **Langages:** PHP, SQL, HTML, CSS
- **Serveur:** Apache (via un installateur MAMP)
- **Database:** MySQL

## Fonctionnalités ajoutées

- [x] refactoring du code existant,
- [x] ajout partout où un utilisateur (auteur, contact, etc) est mentionné d'un lien qui mène vers le mur de cet utilisateur,
- [x] ajout d'une page d'inscription au réseau social,
- [x] ajout d'une page de connexion (avec notions de session),
- [x] ajout d'une page de déconnexion (qui renvoie vers la page login),
- [x] ajout d'un formulaire d’ajout de message quand l'utilisateur est connecté (publication sur son propre mur),
- [x] ajout d'un formulaire d’abonnement / désabonnement sur les murs des autres utilisateurs,
- [x] ajout d'un formulaire pour gérer les likes sur les messages,
- [x] interdictions des pages feed, settings, followers et subscriptions tant que la connexion n’a pas été validée,
- [x] changement du menu profil pour qu’il pointe vers la page de connexion quand l'utilisateur n'est pas connecté,
- [x] séparer les messages en paragraphes (mettre les paragraphes entre balises "p"),
- [x] analyse des #tags (1/2) : lors de la soumission d’un message analyse du texte pour repérer les mots commençant par un dièse "#" et si besoin ajout du mot-clé inconnu dans la table tags,
- [x] utilisation d'une bibliothèque CSS (Bootstrap)

## Reste à implémenter

- [ ] analyse des #tags (2/2) : ajout dans la table posts_tags du lien entre le post et le tag,
- [ ] ajout partout où un mot-clé est mentionné un lien vers la page du mot clé correspondant,
- [ ] permettre à l’utilisateur de “répondre” à un message (à l'aide du champs “parent_id” dans la table “posts” pour noter à quel message correspond cette réponse),
- [ ] permettre le chargement de nouveaux commentaires quand on arrive en fin de page (sans recharger la page) via une bibliothèque javascript comme jquery,
