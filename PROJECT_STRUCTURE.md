# Structure recommandée pour les projets

Ce guide montre les bonnes pratiques pour la structure de vos repositories.

## 📁 Structure projet standard (Python)

```
mon-projet/
├── .github/
│   ├── workflows/              # GitHub Actions CI/CD
│   │   ├── tests.yml
│   │   └── deploy.yml
│   └── ISSUE_TEMPLATE/
├── src/
│   └── mon_module/
│       ├── __init__.py
│       ├── core.py
│       ├── utils.py
│       └── models.py
├── tests/
│   ├── __init__.py
│   ├── test_core.py
│   └── test_utils.py
├── notebooks/
│   └── exploration.ipynb
├── data/
│   ├── raw/                    # Données brutes
│   ├── processed/              # Données traitées
│   └── external/               # Sources externes
├── docs/
│   ├── index.md
│   ├── installation.md
│   └── api.md
├── .gitignore
├── .env.example                 # Template pour variables d'env
├── README.md
├── CONTRIBUTING.md
├── LICENSE
├── requirements.txt
├── setup.py                     # Si publication sur PyPI
└── CHANGELOG.md
```

## 📁 Structure projet React/Next.js

```
mon-app/
├── public/
│   ├── favicon.ico
│   └── images/
├── src/
│   ├── components/
│   │   ├── Header.jsx
│   │   ├── Footer.jsx
│   │   └── common/
│   ├── pages/                  # NextJS
│   │   ├── index.jsx
│   │   └── [id].jsx
│   ├── hooks/
│   │   └── useAuth.js
│   ├── utils/
│   │   └── helpers.js
│   ├── styles/
│   │   └── globals.css
│   └── App.jsx
├── tests/
│   └── __tests__/
├── .env.example
├── .gitignore
├── package.json
├── next.config.js              # Si NextJS
├── README.md
├── CONTRIBUTING.md
└── LICENSE
```

## 📁 Structure Data Science / ML

```
mon-projet-ml/
├── .github/
│   └── workflows/
├── data/
│   ├── raw/
│   ├── processed/
│   └── external/
├── notebooks/
│   ├── 01_exploration.ipynb
│   ├── 02_preprocessing.ipynb
│   ├── 03_modeling.ipynb
│   └── 04_evaluation.ipynb
├── src/
│   └── models/
│       ├── __init__.py
│       ├── train.py
│       ├── predict.py
│       └── evaluate.py
├── models/                      # Modèles entraînés
│   └── model_v1.pkl
├── results/                     # Résultats, métriques
│   └── metrics.json
├── requirements.txt
├── setup.py
├── Makefile                     # Commandes utiles
├── README.md
├── CONTRIBUTING.md
└── LICENSE
```

## 📋 Fichiers essentiels à toujours avoir

### README.md
- Description du projet
- Installation
- Usage/exemples
- TODO/roadmap
- Contributing
- License

### CONTRIBUTING.md
- Comment contribuer
- Setup développement
- Guidelines de code
- Processus de PR

### .gitignore
- Fichiers à ignorer (env, cache, etc.)
- Spécifique à votre stack

### LICENSE
- Choisir une license (MIT, Apache 2.0, GPL, etc.)

### .github/
- Workflows CI/CD
- Templates de issues/PR
- Security policy

## 🎯 Best practices

### 1. Nommage des branches
```
feat/nouvelle-fonctionnalite
fix/correction-bug
hotfix/correction-critique
docs/mise-a-jour-doc
refactor/restructuration
```

### 2. Format des commits
```
feat: brève description
fix: correction de...
docs: documentation de...
style: formatage
refactor: restructuration
test: ajout de tests
chore: maintenance
```

### 3. Versioning (Semantic Versioning)
```
MAJOR.MINOR.PATCH
- MAJOR: changements incompatibles
- MINOR: nouvelles fonctionnalités compatibles
- PATCH: corrections de bugs

Ex: 1.2.3 = major 1, minor 2, patch 3
```

### 4. README sections
```markdown
# Project Name
## Description
## Features
## Installation
## Usage
## Contributing
## License
## Contact
```

### 5. Dépendances
- Garder `requirements.txt` ou `package.json` à jour
- Utiliser `requirements-dev.txt` pour dev
- Pincer les versions critiques

## 🔧 Outils recommandés

### Python
- **Black** - Code formatter
- **Flake8** - Linter
- **pytest** - Testing
- **Sphinx** - Documentation

### JavaScript
- **ESLint** - Linting
- **Prettier** - Formatting
- **Jest** - Testing
- **TypeScript** - Type checking

### Commun
- **Pre-commit** - Git hooks
- **GitHub Actions** - CI/CD
- **Codecov** - Coverage reporting

## 📚 Ressources

- [Keep a Changelog](https://keepachangelog.com/)
- [Semantic Versioning](https://semver.org/)
- [Conventional Commits](https://www.conventionalcommits.org/)
- [GitHub Guidelines](https://docs.github.com/en/github)
- [Python PEP 8](https://www.python.org/dev/peps/pep-0008/)

---

Adaptez cette structure à vos besoins spécifiques ! 🚀
