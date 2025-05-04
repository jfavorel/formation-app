# 🎓 Formation App – Inscription & Interface Admin (React + Node + Docker)

Application web complète pour gérer les inscriptions à une formation via un formulaire public et une interface administrateur protégée.

---

## 🚀 Tech Stack

- **Frontend** : React + Axios + Bootstrap
- **Backend** : Node.js + Express + Sequelize
- **Base de données** : MySQL 8
- **Infrastructure** : Docker + Docker Compose
- **Authentification Admin** : Session Express (login simple)
- **Reverse Proxy possible** : NGINX

---

## 📁 Arborescence

```
formation-app/
├── frontend/          # App React (formulaire, admin UI)
├── backend/           # API Express (routes, contrôleurs, DB)
├── mysql/init.sql     # SQL de création de la DB si besoin
├── docker-compose.yml # Docker multi-services
```

---

## 🔧 Configuration

### 🔐 Variables d’environnement

Créer un fichier `.env` dans `backend/` à partir de `.env.example` :

```bash
cp backend/.env.example backend/.env
```

---

## 🐳 Lancement avec Docker

Dans le dossier `formation-app`, exécute :

```bash
./deploy.sh
```

---

## 🌐 Accès

- **Formulaire public** : `http://<votre-ip>:3000/`
- **Connexion admin**  : `http://<votre-ip>:3000/login`
- **Dashboard admin**  : `http://<votre-ip>:3000/admin`

🧪 **Admin :** `admin` / `1234`

---

## 🧼 .gitignore

- `node_modules`, `build`, `dist`, `.env`, logs, etc.

---

## ✅ Fonctionnalités

- Enregistrement d’un utilisateur
- Affichage des inscrits (admin)
- Suppression d’un inscrit (admin)
- Connexion / déconnexion (admin)
- Responsive et clair (Bootstrap)

---

## 🔐 Sécurité minimale incluse

- Authentification admin (simple)
- Session Express (non JWT)
- `.env` séparé pour secrets

---

## 📦 Dépendances clés

- `express`, `sequelize`, `mysql2`, `cors`, `axios`, `bootstrap`, `react-router-dom`

---

## 🛠️ À faire / évolutions possibles

- Validation serveur plus poussée
- Authentification JWT
- Export CSV
- Pagination admin

---

## ✨ Bravo à vous 👏

Ce projet est prêt à être hébergé sur un VPS Dockerisé.
