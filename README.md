# CP2 — Le Shell

Télécharge le zip depuis le dossier partagé Teams et extrais-le.

```bash
npm install
npm start
```

---

## Mission

Ouvrir `webpack.config.js` et compléter les 3 TODOs :

**TODO 1 — Nommer le Shell**
```js
name: 'shell',
```

**TODO 2 — Préparer les remotes**
```js
remotes: {},
```

**TODO 3 — Partager React**
```js
shared: {
  react: { singleton: true, requiredVersion: '^18.2.0' },
  'react-dom': { singleton: true, requiredVersion: '^18.2.0' },
},
```

---

## Validation

- `npm start` démarre sans erreur
- http://localhost:3000 affiche "Shell opérationnel"
- Push sur `checkpoint2-[nom-equipe]`


## Explication

Le Shell est l’application principale (host) dans une architecture micro-frontend avec Module Federation.
Son rôle est de servir de point d’entrée global, charger dynamiquement les autres applications (remotes) et partager des dépendances communes comme React pour éviter les doublons.
