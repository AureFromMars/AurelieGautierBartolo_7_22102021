# AurelieGautierBartolo_7_22102021 README backend

Ce repository backend est celui du projet 6 du parcours OpenClassrooms Développeur Web.

Outils prérequis :
- Visual Studio Code
- WSL Debian (Windows Subsystem for Linux)
- Commandes de base sous linux

# Installation du backend avec Debian

## 1. Installer de Node.js  
[Documentation](https://github.com/nodesource/distributions/blob/master/README.md)
- Ouvrir une fenêtre VS Code
- Activer WSL Debian (clic sur le logo en bas à gauche WSL : New WSL Window)
- Ouvrir le terminal (comme pour toutes les commandes suivantes)
```
curl -fsSL https://deb.nodesource.com/setup_16.x | bash -

apt-get install -y nodejs
```

## 2. Installer nodemon server  
=> Pour surveiller les modifications de fichiers et éviter d'utiliser systématiquement node server
```
npm install -g nodemon
```
- Remplacer node par nodemon à package.json, et l'exécuter avec npm run start

## 3. Installer le framework Express
[Documentation](http://expressjs.com/fr/)
```
npm install express
```
N.B. Dès Express 4.16, bodyparser est inclu, utiliser expression.json() pour analyser le corps d'une requête  

## 4. Installer le SGBD (Système de Gestion de Bases de Données) 
=> Pour manipuler les données d'une base  
  
### 1. Choix du serveur PostgreSQL
- SQL (Structured Query Language)  
= Langage le plus répandu pour interagir avec les bases de données (imposé par la mission, utilisé chez Calinda Software)
- Choix de l'ORM (Object-Relational Mapping)
= Sequelize de Node  
=> Choix de PostgreSQL, utilisé chez Calinda Software, opensource et suit la syntaxe SQL de très près

### 2. Installer PostgreSQL
[Documentation](https://www.linuxtricks.fr/wiki/debian-10-installer-et-utiliser-postgresql)



