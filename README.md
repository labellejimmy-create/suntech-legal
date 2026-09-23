# suntech-legal

Pages publiques pour l'application interne **SunTech AutoQuote**, hébergées ici afin de fournir les URL publiques exigées par Intuit Developer lors de la demande d'accès à l'API QuickBooks Online (politique de confidentialité, CLUF, et pages du flux de connexion OAuth).

Le code source de l'application reste dans un dépôt privé distinct.

Publié via GitHub Pages : **https://labellejimmy-create.github.io/suntech-legal/**

## Contenu

- [`index.html`](index.html) — page d'accueil
- [`confidentialite.html`](confidentialite.html) — politique de confidentialité
- [`conditions-utilisation.html`](conditions-utilisation.html) — conditions d'utilisation (CLUF)
- [`connexion.html`](connexion.html) — point de départ pour autoriser l'accès QuickBooks (Connect/Reconnect URL)
- [`callback.html`](callback.html) — relaie le `code` et le `state` reçus d'Intuit vers `http://localhost:8000/callback` (Redirect URI de production)
- [`lancement.html`](lancement.html) — confirmation de connexion réussie (Launch URL)
- [`deconnexion.html`](deconnexion.html) — confirmation de révocation de l'accès (Disconnect URL)

`connexion.html` et `callback.html` pointent vers le serveur local de SunTech AutoQuote via une constante `LOCAL` (`http://localhost:8000`) définie dans leur script — à garder cohérente avec le port utilisé par l'application locale.

## Publication

Servi via GitHub Pages (branche `main`, racine `/`), dépôt public : `github.com/labellejimmy-create/suntech-legal`.
