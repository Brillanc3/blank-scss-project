# Project Vierge SCSS

Projet vierge en SCSS pour du mobile-first avec des classes par défaut tel que

- container
- row & size-{1-12} *(pour une grid sur 12 cases)*
- mixins

![CSS Valide](http://jigsaw.w3.org/css-validator/images/vcss)

## Table des matières

- [Pour commencer](#pour-commencer)
- [Utilisation](#utilisation)
  - [Mixins](#mixins)
  - [Fonctions](#fonctions)
- [Auteurs](#auteurs)
- [Licence](#licence)

## Pour commencer

### Prérequis

1. Installer NodeJS : <https://nodejs.org/en/download>

### Installation

1. Intaller le repo :
    - GitHub CLI `gh repo clone Brillanc3/Blank-SCSS-project`
    - HTTPS `git clone https://github.com/Brillanc3/Blank-SCSS-project.git blank_scss_project`
2. Installer les dépendances depuis le dossier racine **blank_scss_project** : `npm install`

## Utilisation

Lancer le serveur local : `npm start`
Retrouver dans le fichier `src\main.scss` les imports des feuilles de style scss

### mixins

#### media queries

```scss
/*
Utilise min-width

Paramètres : 
- breakpoints : sm (576px), md (768px), lg (992px), xl (1200px)
- mediaType : only screen (par default) | Facultatif

*/
@include mq($breakpoints, $mediaType) {
  // Contenu CSS
}
```

#### Racourci CSS

```scss
@include center-fex() // display flex, justify-content: center, align-items: center
@include margin-center($important, $top, $bot) // Défaut : false, 0, 0 
```

### Fonctions

```scss
    // Rien pour le moment
```

## Contribuer

1. Forker le projet
2. Créer une nouvelle branche (`git checkout -b feature/nom-de-la-branche`)
3. Faire les changements nécessaires et les commit (`git commit -am 'Ajouter une fonctionnalité'`)
4. Pousser les changements sur la branche (`git push origin feature/nom-de-la-branche`)
5. Ouvrir une Pull Request

## Auteurs

- Brillance - *Travail initial*

## Licence

[MIT](https://choosealicense.com/licenses/mit/)