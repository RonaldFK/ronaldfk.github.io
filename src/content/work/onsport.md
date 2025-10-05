---
title: On sport
publishDate: 2020-03-04 00:00:00
img: /assets/Deploiement.png
img_alt: architecture
description: |
  Développement du backend d'une application communautaire pour sportifs.
tags:
  - Conception
  - Développeur Backend
---
<h5>Code source</h5>
 <a href="https://github.com/RonaldFK/onsport-backend" style="text-decoration: none; ">Repository</a><br/>
<h5>Contexte du projet</h5>
Onsport est une application communautaire pour sportifs voyageurs qui permet le partage d' activités sportives.<br/>

J'ai travaillé en tant que développeur backend du projet.

<h5>Choix technique</h5>
<table class="styled-table" style="border: 1px solid grey;
  border-collapse: collapse;">
              <thead style="border: 1px solid grey;
  border-collapse: collapse;">
                <tr>
                  <th style="border: 2px solid grey;">Back-End</th>
                  <th style="border: 2px solid grey;">Base de données</th>
                </tr>
              </thead>
              <tbody >
                <tr style="border: 1px solid grey;
  border-collapse: collapse;">
                  <td style="border: 1px solid grey;">
                    <img
                      src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white"
                      alt=""
                    />
                  </td>
                  <td style="border: 1px solid grey;">
                    <img
                      src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white"
                      alt=""
                    />
                  </td>
                </tr>
                <tr style="border: 1px solid grey;
  border-collapse: collapse;">
                  <td style="border: 1px solid grey;">
                    <img
                      src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=grey"
                      alt=""
                    />
                  </td>
                  <td style="border: 1px solid grey;">
                  </td> 
                </tr>
                <tr style="border: 1px solid grey;
  border-collapse: collapse;">
                  <td style="border: 1px solid grey;">
                  <img src="https://img.shields.io/badge/sequelize-323330?style=for-the-badge&logo=sequelize&logoColor=blue">
                  </td>
                  <td style="border: 1px solid grey;"></td>
                </tr>
                <tr style="border: 1px solid grey;
  border-collapse: collapse;">
                  <td style="border: 1px solid grey;">
                    <img
                      src="https://img.shields.io/badge/json%20web%20tokens-323330?style=for-the-badge&logo=json-web-tokens&logoColor=pink"
                      alt=""
                    />
                  </td>
                  <td style="border: 1px solid grey;"></td>
                </tr>
                <tr style="border: 1px solid grey;
  border-collapse: collapse;">
                  <td style="border: 1px solid grey;">Bcrypt</td>
                  <td style="border: 1px solid grey;"></td>
                </tr>
                <tr style="border: 1px solid grey;
  border-collapse: collapse;">
                  <td style="border: 1px solid grey;">Joi</td>
                  <td style="border: 1px solid grey;"></td>
                </tr>
                <tr style="border: 1px solid grey;
  border-collapse: collapse;">
                  <td style="border: 1px solid grey;">Multer</td>
                  <td style="border: 1px solid grey;"></td>
                </tr>
              </tbody>
            </table>
            </br>

<h5>Développement</h5>
Sur la première phase de développement, il a été nécessaire de travailler avec l'API des communes de France.</br>

Ce type de données ne changeant que très rarement, le choix a été fait d'intégrer les données souhaitées dans la base de l'application.</br>

Voici la roadmap qui a été suivi pour le développement des fonctionnalités: 

<ol>
<li>Authentification</li>
<li>Développement des routes nécessaires par ordre de priorité</li>
<li>Intégration de middleware pour la gestion des erreurs et conflits</li>
<li>Déploiement distant en HTTP</li>
<li>Rajout de Jason Web Token</li>
<li>Déploiement distant avec certificat SSL ( NGINX / Lets'sEncrypt )</li>
</ol>

<h5>Fonctionnalités interessantes / Difficultés</h5>

- L'une des fonctionnalités intéressantes à implémenter sur ce projet a été la gestion de la photo de profil utilisateur.</br>
Il a nécessaire de gérer le fait de remplacer la photo existante de l'utilisateur s'il en existe une, mais également de supprimer celle-ci du serveur distant pour des questions de confidentialité.
<img src="/assets/profilProcess.png">
</br>

- La suppression d'un profil utilisateur a également fait l'objet d'une réflexion.
En effet, un utilisateur peut ajouter un commentaire et noter une activité, ainsi que lui-même en créer.</br>
Afin de conserver toutes ces données et surtout que la suppression d'un profil n'impacte pas l'évaluation des activités, il a été décidé - lors de la demande de suppression du compte utilisateur => d'anonymiser ses données en base => supprimer sa photo de profil du serveur distant => renommer son profil et ses données sensibles.</br>
Cela permet de conserver une trace au niveau des commentaires et des notes utilisateurs.
</br>

- J'avais également pour mission le déploiement sécurisé de l'application sur le serveur distant.</br>

Pour cela, j'ai d'abord procédé par la création d'un certificat SSL avec Lets'Encrypt, puis paramétré le backend afin de créer un serveur en HTTPS.</br>

Cela permet de communiquer de manière sécurisé du front vers le back.
J'ai donc configuré deux serveurs - l'HTTP étant pour les besoins en développement.
<img src="/assets/sslConfig.png">
<h5>Démo</h5>
					<div class="stack gap-10 content">
          <video controls >
          <source src="/assets/onSport.mov" type="video/mp4">
</video>
					</div>