# Cronexia-front

## Execution du code

Node.JS version used: v18.18.0. It can simply be installed through `nvm install && nvm use` or in any method of your choice if you don't use nvm.

- First run:
	- `npm install`
	- `npx tsc`

## Front end:
- `npm run server`: The website can be accessible through `http://localhost:5000/`. There is honnestly nothing to see.

# Reponse théorique:

1. Le FOUC est le fait qu'une page puisse s'afficher à l'utilisateur avant que les fichiers de style ne soient reçus par le client. Ce qui résulte, en bref, un affichage sans style et très sommaire.
Un des moyens d'empêcher le FOUC est d'éviter d'afficher le contenu de la page tant que les fichiers de style ne sont pas reçus par le serveur.
Il existe pour cela des événements associés au DOM de la page, étant émis quand ce dernier est prêt, qui peuvent permettre via script d'afficher le contenu seulement quand ce dernier est prêt.

2. Je n'ai à ce jour que rencontré l'utilisation du composant `Suspense` permettant, lors d'un chargement d'un fort contenu, d'afficher un composant plus léger et rapide le temps que le tout puisse être chargé et affiché.
