# Contributing Guide / Guide de Contribution

Merci d'être intéressé par la contribution à mes projets ! 🙏

## 📋 Avant de commencer

- Vérifiez les **issues ouvertes** pour éviter les doublons
- Consultez le **README.md** du projet pour comprendre le contexte
- Assurez-vous que votre contribution s'aligne avec les objectifs du projet

## 🔄 Workflow de contribution

### 1. Fork le repository
```bash
# Cliquez sur "Fork" sur la page du repository
```

### 2. Créez votre branche
```bash
git checkout -b feature/ma-fonctionnalite
# ou
git checkout -b bugfix/correction-probleme
```

### 3. Développez votre changement
- Écrivez du code propre et lisible
- Ajoutez des tests si applicable
- Commentez votre code si nécessaire

### 4. Testez votre code
```bash
# Selon le langage/projet
pytest              # Python
npm test           # JavaScript
```

### 5. Commit et Push
```bash
git commit -m "feat: description claire de vos changements"
git push origin feature/ma-fonctionnalite
```

### 6. Créez une Pull Request
- Décrivez clairement vos changements
- Référencez les issues associées (#XXX)
- Expliquez pourquoi ces changements sont nécessaires

## 📝 Guidelines de commit

Utilisez les [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: nouvelle fonctionnalité
fix: correction de bug
docs: documentation
style: formatage, lint
refactor: restructuration sans changement fonctionnel
test: ajout/modification de tests
chore: tâches de maintenance
```

Exemple:
```
feat: ajout de la prédiction de consommation énergétique
fix: correction du bug de chargement du modèle
docs: mise à jour du README
```

## ⚙️ Setup du développement

### Requirements généraux
- Python 3.8+
- Node.js 16+ (si applicable)
- Git

### Installation locale
```bash
# Clone votre fork
git clone https://github.com/YOUR_USERNAME/repository.git
cd repository

# Créez un environnement virtuel (Python)
python -m venv venv
source venv/Scripts/activate  # Windows
# ou
source venv/bin/activate     # Linux/Mac

# Installez les dépendances
pip install -r requirements.txt
# ou
npm install
```

## 🧪 Tests

Tous les changements doivent passer les tests :

```bash
# Python
pytest
pytest --cov          # Avec coverage

# JavaScript
npm test
npm run lint
```

## 📚 Ressources

- [Documentation Python](https://docs.python.org/)
- [React Documentation](https://react.dev/)
- [Git Documentation](https://git-scm.com/doc)

## 🤝 Code of Conduct

- Soyez respectueux envers tous les contributeurs
- Pas de spam, harcèlement ou comportement abusif
- Restez professionnel dans vos communications
- Accueillez les critiques constructives

## ❓ Questions ?

- Ouvrez une **Issue** pour les questions
- Consultez les **Discussions** existantes
- Contactez-moi via mon profil GitHub

---

Merci de contribuer ! 🚀
