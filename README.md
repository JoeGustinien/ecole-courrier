# Courriers parents d'élèves — Saint-Denis 93

Site statique permettant aux parents d'élèves de l'école élémentaire Maria Casares et du groupe scolaire Doisneau Casares (Saint-Denis) de générer rapidement un courrier électronique pré-rédigé à destination de l'académie et des associations de parents.

## Fonctionnalités

- **3 modes de rédaction** : deux situations pré-rédigées + un éditeur libre
  - Fermetures de classes et baisses de dotation horaire (rentrée 2026)
  - Demande urgente de remplacement d'un professeur absent
  - Mail libre (objet et corps entièrement personnalisables)
- **Destinataires pré-renseignés** : DSDEN 93, FCPE Saint-Denis, direction des deux établissements
- **Texte modifiable** avant envoi directement dans le navigateur
- **Ouverture en un clic** dans le client mail du parent (Gmail, Apple Mail, Outlook…) via `mailto:`
- **QR code** généré côté client — sur smartphone, scanner ouvre directement l'application mail
- **Lien court** généré via l'API is.gd, pointant vers la page avec la situation pré-sélectionnée

## Stack technique

- HTML / CSS / JavaScript vanilla — aucun framework, aucun serveur
- [qrcode.js](https://github.com/davidshimjs/qrcodejs) via CDN pour la génération du QR code
- API [is.gd](https://is.gd) pour le raccourcissement d'URL
- Déployé sur [Netlify](https://netlify.com) (déploiement continu depuis GitHub)

## Destinataires

| Organisme | Adresse |
|---|---|
| DSDEN 93 | ce.dsden93@ac-creteil.fr |
| FCPE Saint-Denis | contact@fcpe-saint-denis.org |
| École Doisneau | ce.0931037x@ac-creteil.fr |
| École Casares | ce.0931036W@ac-creteil.fr |

## Utilisation locale

Aucune installation requise. Ouvrir `index.html` directement dans un navigateur.

## Déploiement

Le site est déployé automatiquement sur Netlify à chaque push sur la branche `main`.
