
# Plateforme AfricTivistes CitizenLab

## Aperçu
Ce dépôt contient l'architecture monorepo de la plateforme AfricTivistes CitizenLab, une plateforme web centralisée conçue pour soutenir et autonomiser les acteurs de la société civile dans divers pays africains.

## Structure du Projet
```
├── packages/
│   └── astrowind/           # Package du thème de base
├── sites/
│   └── citizenlab/          # Application principale CitizenLab
└── pnpm-workspace.yaml      # Configuration de l'espace de travail
```

## Pourquoi un Monorepo ?

Notre architecture monorepo sert plusieurs objectifs clés :

1. **Composants Partagés** : Le dossier `packages/astrowind` contient notre thème de base et les composants partagés qui peuvent être réutilisés dans les différents sites spécifiques à chaque pays.

2. **Développement Cohérent** : L'utilisation d'un monorepo assure des pratiques de développement et des outils cohérents pour tous les sites.

3. **Évolutivité** : Facilité d'ajout de nouveaux sites spécifiques aux pays tout en maintenant la cohérence et la réutilisabilité du code.

## Stack Technologique

- **Framework** : Astro 5.0 avec Tailwind CSS
- **Gestionnaire de Paquets** : pnpm avec support workspace
- **Outil de Build** : Turborepo pour un système de build efficace

## Fonctionnalités Principales

- Architecture multi-sites supportant les sous-domaines par pays
- Gestion centralisée des ressources
- Support multilingue
- Design responsive
- Système de gestion de blog et de contenu
- Optimisation SEO

## Démarrage

1. Installer les dépendances :
```bash
pnpm install
```

2. Démarrer le serveur de développement :
```bash
pnpm dev
```

3. Construire pour la production :
```bash
pnpm build
```

## Contribution

Veuillez suivre nos directives de développement lors de la contribution au projet. Chaque site spécifique à un pays doit être ajouté sous le répertoire `sites/` en suivant les modèles établis.

## Licence

[Licence MIT](LICENSE)
