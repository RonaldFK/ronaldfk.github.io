---
title: Club de tennis
publishDate: 2020-03-04 00:00:00
img: /assets/sql.png
img_alt: architecture
description: |
  Projet SQL - application club de tennis.
tags:
  - Conception
  - SQL
---
<h5>Code source</h5>
 <a href="https://github.com/RonaldFK/InitDatabase-no-ORMapp" style="text-decoration: none; ">Repository</a><br/>
<h5>Contexte du projet</h5>
Ce projet SQL vient déplacer au niveau de la base de données les fonctionnalités CRUD.</br>
Côté serveur, le développeur devra exécuter ces fonctions afin d'effectuer une action.



<h5>Choix technique</h5>

- PostgresSQL pour le stockage des données de l'application.
- Docker pour exécuter notre conteneur Postgres.
- PGAdmin.
- DOMAIN pour la création de type de données générique afin de rajouter un contrôle sur les emails notamment avec un REGEX.
</br>

<h5>Développement</h5>
Au moment de l'initialisation, je créé également les types de données(DOMAINS) que j'utilise par la suite pour valider le format de données que j'attends.

Ici, par exemple, la création de deux domains qui permettrons de valider le format de donnnées pour le nom et l'adresse email.

<img src="/assets/domains.png">



<h5>Démo</h5>
					<div class="stack gap-10 content">
          <video controls >
          <source src="/assets/tennisClub.mov" type="video/mp4">
</video>
					</div>