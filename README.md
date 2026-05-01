# Blog

Journal de bord sur l'application des principes SRE à un indexeur Uniswap V4.

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
    ├── api/               # Endpoints API (SSR)
    ├── articles/
    │   └── [slug].astro   # Page article
    ├── index.astro        # Liste des articles
    └── ressources.astro   # Page ressources
```

## Lancer Astro

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

