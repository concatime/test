# Important

Les commandes doivent être exécutées dans `client` ou `server`.

## Installation des dépendances

- `npm install`

## Développement de l'application

Pour le serveur, `npm run build` transpile le TypeScript, et `npm start` exécute
le JavaScript en continu. `npm run watch` permet d’auto-transpiler à chaque
modification de code.

## Génération de composants du client

`ng generate component <name>` crée un component.

Il est aussi possible de générer des directives, pipes, services, guards, interfaces, enums, muodules, classes, avec cette commande `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Exécution des tests unitaires

- `npm t` exécute les test

- `npm run coverage` génére un rapport de couverture de code

## Exécution de ESLint/TSLint

- `npm run lint` exécute ESLint pour le serveur et TSLint pour le client

## Documentation externe

- [Angular CLI README](//github.com/angular/angular-cli/blob/master/README.md)
  (ou `ng help`)

- [Angular Testing](//angular.io/guide/testing)

- [Angular](//angular.io/docs)

- [Express](//expressjs.com/en/4x/api.html)

- [Mongo](//docs.mongodb.com/manual/)

# Standards de programmations

Cette section présente les différents standards de programmations que vous devez
respecter lors de la réalisation de ce projet et qui seront utilisés pour la
correction de l'assurance qualité de votre projet.

## Format

Une ligne de code ne devrait JAMAIS dépasser les 80 caractères (par défaut dans
ESLint](//eslint.org/docs/rules/max-len#options)).

TODO: ME DEBARASSER DE CETTE CONFIG

Voici les configurations pour le formateur de code `Prettier`. Ajoutez tout ce qui est à l'intérieur de `{ }` dans le `settings.json` de votre VSCode.

```json
{
    "prettier.printWidth": 120,
    "prettier.tabWidth": 4,
    "prettier.trailingComma": "all",
    "prettier.arrowParens": "always",
    "prettier.disableLanguages": [],
    "prettier.singleQuote": true,
    "prettier.endOfLine": "lf",
    "[javascript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[html]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[typescript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[json]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    }
}
```

## Conventions de nommage

- UPPER\_SNAKE\_CASE pour les constantes.

- PascalCase pour les noms de types et les valeurs d'énumérations.

- camelCase pour les noms de fonctions, de propriétés et de variables.

- kebab-case pour les noms de balises des composants Angular.

- Évitez les abbréviations dans les noms de variables ou de fonctions.

- Un tableau/list/dictionnaire devrait avoir un nom indiquant qu'il contient
  plusieurs objets, par exemple "cars".

- On évite de mettre le type de l'objet dans le noms, par exemple on préfère
  “cars” à “listOfCars” lorsqu’on déclare une liste.

- Nous devons coder en anglais.

## Autres standards

- N'utilisez jamais var. Utilisez let et const.

- N'utilisez jamais any et object, que ce soit implicitement ou explicitement.

- N'utilisez pas le mot-clé function, utilisez les fonctions anonymes: `() => {...}`.

- Déclarez tous les types de retour des fonctions (incluant void) et les type de paramètres.

- Évitez les fonctions qui ont plus d'une responsabilité et pas d'overloading.

- N'utilisez pas de nombres magiques.

- N'utilisez pas de chaînes de caractères magiques. Créez vos propres constantes avec des noms explicites.

- Une fonction devrait avoir 4 paramètres ou moins.

- Séparez votre code Typescript du CSS et du HTML. Générez vos component avec Angular CLI qui le fait pour vous.

## Git

- Une seule fonctionnalité par branche.

- Une branche fonctionnalité devrait se nommer `fonctionnalite/nom-de-la-fonctionnalite`.

- Une branche correction de bogue devrait se nommer `boggefixe/nom-du-bogge`.

- Les messages de commit doivent être concis et significatifs. Ne mettez pas des messages trop long ou trop courts. On devrait être capable de comprendre ce que le commit fait sans lire les changements.

- Les commits doivent être ecrit en francais et au présent.

```

```

<!--
vim:cc=80:tw=80:fo+=a
-->
