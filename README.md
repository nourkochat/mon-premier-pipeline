# Mon Premier Pipeline CI/CD

## 📋 Description
Projet de démonstration de CI/CD avec GitHub Actions et Docker.
Réalisé dans le cadre du TP5 de Génie Logiciel.

## 🌐 URLs
- **Site GitHub Pages** : https://nourkochat.github.io/mon-premier-pipeline/
- **Dépôt GitHub** : https://github.com/nourkochat/mon-premier-pipeline

## 🔄 Workflows
1. **CI - HTML Validation** : Valide la syntaxe HTML à chaque push
2. **CD - GitHub Pages** : Déploie automatiquement sur GitHub Pages
3. **Docker CI** : Construit et teste l'image Docker

## 🐳 Commandes Docker utilisées
\\\ash
# Construire l'image
docker build -t mon-site .

# Lancer le conteneur
docker run -d -p 8080:80 --name mon-site-container mon-site

# Vérifier les conteneurs actifs
docker ps

# Arrêter le conteneur
docker stop mon-site-container

# Supprimer le conteneur
docker rm mon-site-container
\\\

## 📁 Structure du projet
\\\
mon-premier-pipeline/
├── .github/
│   └── workflows/
│       ├── ci.yml           # Validation HTML
│       ├── cd.yml           # Déploiement GitHub Pages
│       └── docker-ci.yml    # CI Docker
├── index.html               # Page web
├── Dockerfile               # Configuration Docker
└── README.md                # Documentation
\\\

## 👤 Auteur
**Nour Kochat**  
TP Génie Logiciel - Classe 2LM  
A.U : 2024/2025

## 📚 Technologies utilisées
- Git & GitHub
- GitHub Actions
- Docker
- Nginx
- HTML5
