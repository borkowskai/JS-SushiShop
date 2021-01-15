## First exercices of JavaScript without using HTML

- CSS is allowed

**The idea is :**
- to make appear data with 100% JavaScript 
- make the functional basket in JavaScript

## Setup
To open a project you need node module:

```
npm install
npm start
```

## Steps of exercice

Pour cette exercice, vous avez droit a toutes les sources d'information, mais pas à la communication.

Les copier/coller de code d'internet seront sanctionné.

Dans `./src/data/makis.js`, une liste de makis japonais est exportée.

- Ajouter des makis à cette listes sur le même modèle (avocat, concombre, omelette).

Dans `./public/index.html` (la page d'accueil) il y une `div` a l'id `app`. Le script `./src/index.js` est déjà lié à cette page grâce à webpack.

L'exercice est la création dynamique d'un magasin en ligne de maki (type Makisu ou Sushishop).

Sans JAMAIS toucher le HTML:

- présentez la carte des makis et toutes leurs infos utiles dans la page d'accueil.
- le prix d'un seul maki est donné dans la liste, mais les makis se vendent par 8: affichez ce nombre et le prix correct dans votre HTML.
- Dans le header, un maki pris au hasard est mis en avant (une simple copie de celui de la carte)
- Chaque boite de 8 makis a un bouton "acheter"
- Dans le footer de la page, il y a un panier (vide au début). Il ne présentera que le nom et le prix des makis réservés, ainsi que le prix total de la commande et un bouton "commander"
- On peut aussi supprimer un maki avant la commande
- lorqu'on clic sur un bouton "acheter", une copie du maki est mis dans le panier
- Lorqu'on clic sur "commander" dans le footer, la page entière se vide, et affiche "Votre commande est en cours de livraison. Elle arrivera dans `x` minutes", ou `x` est le nombre de boite de maxi \* 6.

Bonus (pas compté dans le points, sauf en bonus):
- Améliorer l'affichage de votre site grâce au css
- Mettez les makis dans un fichier JSON valide, dans les assets, et requêtez le avec `fetch` ou `axios` au début du code
- Un bouton permet de vider tout le panier
- Les sushis végétariens ont une bordure verte
- Si l'utilisateur achète plus de 50€ de sushi, il a un discount de 20% sur sa commande
