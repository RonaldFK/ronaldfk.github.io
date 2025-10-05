---
title: Immo App
publishDate: 2020-03-04 00:00:00
img: /assets/architecture.png
img_alt: architecture
description: |
  Développement d'une application de gestion de biens immobiliers.
tags:
  - Conception
  - Développeur FullStack
---
<h5>Code source</h5>
 <a href="https://github.com/RonaldFK/api-immo" style="text-decoration: none; ">Repository Back End</a><br/>
 <a href="https://github.com/RonaldFK/font-immo" style="text-decoration: none;">Repository Front End</a>
<h5>Contexte du projet</h5>
Le but de ce projet était principalement de me permettre de monter en compétence sur la technologie typescript et de prendre en main un framework front-end comme Vue Js.<br/>
Partant du besoin d'une agence immobilière qui souhaite pouvoir gérer ses biens dans un logiciel métier, j'ai commencé ce projet dans le but de sortir un MVP qui puisse répondre à ce besoin.

<h5>Choix technique</h5>
<table class="styled-table" style="border: 1px solid grey;
  border-collapse: collapse;">
              <thead style="border: 1px solid grey;
  border-collapse: collapse;">
                <tr >
                  <th style="border: 2px solid grey;">Front-End</th>
                  <th style="border: 2px solid grey;">Back-End</th>
                  <th style="border: 2px solid grey;">Base de données</th>
                </tr>
              </thead>
              <tbody >
                <tr style="border: 1px solid grey;
  border-collapse: collapse;">
                  <td style="border: 1px solid grey;">
                    <img
                      src="https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vue.js&logoColor=4FC08D"
                      alt=""  
                    />
                  </td>
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
                  <td style="border: 1px solid grey;">Vue Router</td>
                  <td style="border: 1px solid grey;">
                    <img
                      src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white"
                      alt=""
                    />
                  </td>
                  <td style="border: 1px solid grey;">Table virtuelle(view)</td>
                </tr>
                <tr style="border: 1px solid grey;
  border-collapse: collapse;"> 
                  <td style="border: 1px solid grey;">
                    <img
                      src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=grey"
                      alt=""
                    />
                  </td>
                  <td style="border: 1px solid grey;">TypeOrm</td>
                  <td style="border: 1px solid grey;"></td>
                </tr>
                <tr style="border: 1px solid grey;
  border-collapse: collapse;">
                  <td style="border: 1px solid grey;">Vuetify</td>
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
                  <td style="border: 1px solid grey;">Fetch</td>
                  <td style="border: 1px solid grey;">Bcrypt</td>
                  <td style="border: 1px solid grey;"></td>
                </tr>
                <tr style="border: 1px solid grey;
  border-collapse: collapse;">
                  <td style="border: 1px solid grey;">Chart JS</td>
                  <td style="border: 1px solid grey;">Joi</td>
                  <td style="border: 1px solid grey;"></td>
                </tr>
                <tr style="border: 1px solid grey;
  border-collapse: collapse;">
                  <td style="border: 1px solid grey;"></td>
                  <td style="border: 1px solid grey;">Multer</td>
                  <td style="border: 1px solid grey;"></td>
                </tr>
              </tbody>
            </table>
            </br>
Pour le choix technique de ce projet, j'avais trois technologies sur lesquelles je souhaitais me former et donc que j'ai intégré.</br>

- TypeORM
- Typescript.
- Vuejs.
<h5>Développement</h5>
J'ai commencé ce projet en me formant sur typescript que j'ai ensuite utilisé pour le développement de la partie serveur.</br>

Suite à cela, j'ai commencé par noter les besoins exacts auxquels le logiciel devra répondre dans sa V1 afin de poursuivre avec la partie conception de base de données</br>
</br>
Une fois la partie serveur terminée et testée avec postman, j'ai pu me focaliser sur la partie front end toujours en commençant par me former sur le fonctionnement d'un framework front end et donc de Vuejs.
</br>
<h5>Fonctionnalités interessantes / Difficultés</h5>
Sur ce projet, j'ai souhaité mettre en place un graphique avec Chart JS afin de permettre de visualiser le nombre de biens rentrés à l'agence et le nombre de biens vendus par mois.</br>
Ce fut une fonctionnalité interessante à implémenter, car j'ai dû créer une route spécifique côté serveur et réfléchir à comment bien implémenter cette fonction.</br>
La problématique principale ici a été la prise en compte que sur une année complète, il était possible d'avoir des données de manière complètement aléatoire ( exemple : l'agence a vendu des biens en Janvier, Juillet et Septembre uniquement )</br>
<h5>Piste de fonctionnalités</h5>
<ul>
<li>Rajouter une validation par mail avant création effective du compte ou d'une page admin</li>
<li>Prendre en compte les locataires si c'est le cas pour certains biens</li>
</ul>


<h5>Démo</h5>
					<div class="stack gap-10 content">
          <video controls >
          <source src="/assets/demo_immo480.mov" type="video/mp4">
</video>
					</div>