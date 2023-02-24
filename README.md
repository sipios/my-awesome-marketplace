# Dojo fintech Sipios

Le CEO de _Skin My Life_ commence à se poser des questions. Pourquoi son concurrent _Skin me_ fait-il autant de ventes ? Apres avoir fait appel à un cabinet de conseil en stratégie, il découvre que le concurrent permet à ses clients non seulement de payer avec le moyen de leur choix mais en plus ces paiements sont complètements déplafonnés. Un avantage conséquent lorsqu’il s’agit d’acheter plusieurs **skins** ou **Add on**...

Après une réunion avec KO-BC, _Skin My Life_ vous missione pour créer une interface web plus poussée en utilisant l’API de paiement Siprip de KO-BC avec qui il vient de faire affaire. Tu l’as compris, plus les joueurs peuvent dépenser par achat, plus tu permettras à _Skin My Life_ de rattraper son retard.

## Le but du jeu

Le but du jeu est de généré le plus gros chiffre d'affaire.
Vous êtes mis en concurrence entre vous et vous pouvez consulter le classement en suivant ce [lien](https:// ).
Le gagant est le joueur qui aura généré le plus gros chiffre d'affaire d'ici la fin de la session.

## Les règles du jeu

Tu peux utiliser cette base de code d'une application React.js pour développer ta marketplace. Tu as accès à un catalogue de 50 skins. Ton objectif est de mettre en place le moyen de paiement pour chaque skin.

***/!\ Attention /!\*** il y a plusieurs niveaux de difficulté.

Tu ne peux pas acheter une skin tant que tu n'as pas débloqué de niveau suivant :
- Niveau 1 : Carte cadeau PSN inférieur ou égal à 10€ avec 1 achat tous les 10 minutes
- Niveau 2 : Ticket PSN inférieur ou égal à 50€  avec 1 achat tous les 5 minutes
- Niveau 3 : Paypal inférieur ou égal à 1000€ avec 1 achat par minute
- Niveau 4 : Carte bancaire déplafonné avec achat illimité

## Pré-requis

Afin de jouer, tu as besoin d'une API key qui te sera envoyée par email lors de ton enregistrement.

Suis les intructions sur cette [page](https:// ) pour t'enregistrer et recevoir ton API key.
Une fois obtenue, tu dois créer un fichier _.env.local_ à la racine de ce projet et ajouter une ligne avec ta clé en suivant cette syntaxe :
```
VITE_PLAYER_TOKEN=<TON API KEY>
```

### Dépendances javascript

Tu dois tout d'abord installer les dépendance javascript pour pouvoir exécuter ton projet en local sur ton poste.
Pour ce faire lance la commande :
```shell
$ npm ci
```

Un dossier _node_modules_ va être créé avec toutes les dépendances téléchargées à l'intérieur.

### Lancer le projet

Pour lancer ton application tu peux utiliser la commande :
```
$ npm run dev
````
Un serveur local va distribuer ton application que tu peux consulter sur le lien [http://127.0.0.1:5173](http://127.0.0.1:5173).
Si tu as bien saisie ton API key, un catalogue de 50 skins s'affiche après un court temps de chargement.

## L'API Siprip

Tu vas consommer l'API de Siprip pour effectuer les paiements.
Tu trouveras la documentation de cette API en suivant ce [lien](https:// ).

Certaines routes ne sont pas documentés (volontairement) et c'est à toi de les découvrir pour passer les niveaux.

Good Luck, Have Fun (GL HF) !!