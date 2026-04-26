# indexer.blog — Journal de bord SRE

Journal de bord sur l'application des principes SRE à un indexeur Uniswap V4.
Le gap entre la théorie SRE et une infrastructure blockchain qui tient en production.

## Stack

- **Frontend** : Astro (SSR)
- **Backend / CMS** : PocketBase
- **Styles** : CSS vanilla, JetBrains Mono
- **Déploiement** : Docker

## Structure

```
src/
├── layouts/
│   └── Layout.astro       # Layout global (nav, footer)
├── lib/
│   └── pocketbase.ts      # Client PocketBase
└── pages/
    ├── index.astro         # Liste des articles
    └── articles/
        └── [slug].astro    # Page article
```

## Lancer le frontend Astro

```sh
npm install
npm run dev       # http://localhost:4321
npm run build
npm run preview
```

## Lancer Pocketbase

```sh
.\pocketbase.exe serve     
```

## Auteur

Hugo GERARD

