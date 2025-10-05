---
title: Module d'authentification
publishDate: 2020-03-04 00:00:00
img: /assets/archiAuth.png
img_alt: architecture
description: |
  Développement d'un module d'authentification.
tags:
  - Conception
  - Développeur Backend
---
<h5>Code source</h5>
 <a href="https://github.com/RonaldFK/authentification" style="text-decoration: none; ">Repository</a><br/>
<h5>Contexte du projet</h5>
Projet de gestion de l'authentification - formulaire d'inscription et de connexion.

L'idée est de créer un module de gestion de l'authentification.


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
                  <img
                      src="
                https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white"
                      alt=""
                    />
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
                                <tr style="border: 1px solid grey;
  border-collapse: collapse;">
                  <td style="border: 1px solid grey;">NodeMailer</td>
                  <td style="border: 1px solid grey;"></td>
                </tr>
              </tbody>
            </table>
            </br>
Ce projet utilise deux bases de données.</br>
L'idée est d'utiliser la base de données Portgresql afin de stocker les données métiers et mongoDB pour le stockage et la gestion des sessions.</br></br>
Le but était de comprendre comment pouvait se structurer le back End en utilisant deux sources de données différentes et appliquer le principe de séparation des concepts aux données de type session.
<h5>Développement</h5>
La phase de développement se concentre sur la fonction d'authentification et le stockage des sessions lors de la validation d'une connexion.</br>

J'ai pris de temps de lire quelques articles sur les bonnes pratiques et le stockage des sessions dans une application, car je me posais effectivement la question sur la pertinence de stocker les sessions utilisateurs dans la même base de données qui contient les données métiers.</br>

Le point qui remonte notament ici, est le coût que cela peut avoir d'utiliser deux bases de données différentes pour une application.</br>

Ici, je n'ai pas pris en compte l'aspect financier pour ce projet - le but étant surtout de me focaliser sur l'aspect technique.

<h5>Fonctionnalités interessantes / Difficultés</h5>
Ce projet m'a permis de mieux comprendre comment peut s'intégrer plusieurs sources de données dans une application côté serveur.

<h5>Démo</h5>
					<div class="stack gap-10 content">
          <video controls >
          <source src="/assets/goodTest.mp4" type="video/mp4">
</video>
					</div>