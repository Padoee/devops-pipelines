# 🚀 DevOps Pipelines

Petit projet Node.js créé pour **apprendre et expérimenter les pipelines CI/CD** avec GitHub Actions.

[![CI Pipeline](https://github.com/Padoee/devops-pipelines/actions/workflows/pipeline.yaml/badge.svg)](https://github.com/Padoee/devops-pipelines/actions/workflows/pipeline.yaml)
![Node](https://img.shields.io/badge/node-16-green)
![License](https://img.shields.io/badge/license-ISC-blue)

---

## 📖 Description

Ce dépôt sert de bac à sable pour comprendre le fonctionnement d'une pipeline d'intégration continue :
- installation des dépendances,
- exécution automatique des tests,
- déclenchement automatique à chaque `push` sur `main`.

## 📂 Structure du projet

```
devops-pipelines/
├── .github/
│   └── workflows/
│       └── pipeline.yaml   # Configuration GitHub Actions (CI)
├── index.js                # Point d'entrée de l'application
├── test.js                 # Script de test
├── package.json            # Dépendances et scripts npm
└── README.md
```

## ⚙️ Prérequis

- [Node.js](https://nodejs.org/) v16 ou supérieur
- npm

## 🛠️ Installation

```bash
git clone https://github.com/Padoee/devops-pipelines.git
cd devops-pipelines
npm install
```

## ▶️ Utilisation

Lancer l'application :

```bash
npm run run
```

Lancer les tests :

```bash
npm test
```

## 🔄 Pipeline CI/CD

Le workflow `.github/workflows/pipeline.yaml` s'exécute automatiquement à chaque `push` sur la branche `main` et effectue les étapes suivantes :

1. **Checkout** du code source
2. **Installation** de Node.js (v16)
3. **Installation** des dépendances (`npm install`)
4. **Exécution** des tests (`npm test`)

## 🗺️ Roadmap

- [ ] Ajouter un vrai jeu de tests (Jest/Mocha)
- [ ] Ajouter un job de lint
- [ ] Ajouter un déploiement automatique

## 📄 Licence

Ce projet est sous licence **ISC**.

## 👤 Auteur

[Padoee](https://github.com/Padoee)
