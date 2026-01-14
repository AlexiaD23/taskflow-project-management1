# 🚀 TaskFlow v1.0 - Sistem de Management al Sarcinilor

ACCESEAZA APLICATIA AICI:  https://taskflow-project-management1.vercel.app/

TaskFlow este o aplicație web modernă pentru gestionarea fluxurilor de lucru în cadrul unei organizații, construită pe arhitectura **Client-Server**. Aplicația permite coordonarea eficientă între Administratori, Manageri și Executanți.

## 🛠️ Tehnologii Utilizate

* **Frontend:** React.js, Axios, React Router v6.
* **Backend:** Node.js, Express.js.
* **Bază de Date:** PostgreSQL / MySQL (via Sequelize ORM).
* **Autentificare:** JSON Web Tokens (JWT) & BcryptJS.
* **Design:** Custom CSS (Premium Clean UI - Stil Jira/Asana).

## 📋 Funcționalități Principale

### 🛡️ Administrator
* Crearea utilizatorilor noi (Manageri sau Executanți).
* Configurarea ierarhiei (alocarea executanților către manageri).

### 👔 Manager
* Crearea și gestionarea proiectelor.
* Lansarea sarcinilor noi (**OPEN**).
* Alocarea sarcinilor către subordonați directi (**PENDING**).
* Monitorizarea echipei în timp real (Tab-ul Team).
* Închiderea definitivă a sarcinilor finalizate (**CLOSED**).
* Filtrarea și consultarea istoricului pe fiecare executant.

### 👷 Executant
* Vizualizarea sarcinilor alocate personal.
* Marcarea sarcinilor ca realizate (**COMPLETED**).
* Acces la istoricul personal de activitate.

## 🚀 Instalare și Configurare

### 1. Clonare proiect
```bash
git clone [https://github.com/utilizator/taskflow.git](https://github.com/utilizator/taskflow.git)
cd taskflow

2. Configurare Backend
 # Navighează în folderul serverului
cd backend

# Instalează dependențele (Express, Sequelize, JWT, Bcrypt)
npm install

3. Configurare Frontend
# Navighează în folderul clientului
cd frontend

# Instalează bibliotecile necesare (React Router, Axios)
npm install

Conexiunea cu API-ul: Aplicația folosește variabila API_URL pentru a comunica cu backend-ul de pe Render.

Producție: https://taskflow-api-qkmb.onrender.com/api

Local: http://localhost:8080/api

Pornire and deploy:
# Dezvoltare locală
npm start

# Deploy via Vercel CLI (sau automat prin GitHub Integration)
vercel deploy

Aplicația utilizează o strategie de tip Cross-Platform Hosting:

Backend (Node.js/Express): Găzduit pe Render.com (Web Service).

Bază de Date (PostgreSQL): Găzduită pe Clever Cloud.

Frontend (React): Găzduit pe Vercel pentru performanță maximă și SSL automat.
