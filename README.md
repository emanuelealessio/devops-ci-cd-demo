# 🚀 DevOps Project: CI/CD with GitHub Actions + Docker

Questo progetto dimostra una pipeline CI/CD utilizzando **GitHub Actions** per:
- Costruire un'immagine Docker
- Spingerla automaticamente su **Docker Hub**

## 📦 Struttura del progetto

📁 .github/workflows/
└── ci-cd.yml # Workflow GitHub Actions
📄 Dockerfile # Costruisce l'immagine
📄 app.py / main.js # Codice dell'app (es. web server minimale)
📄 README.md # Questo file

## ⚙️ Tecnologie usate

- **GitHub Actions** – CI/CD automation
- **Docker** – containerizzazione dell'app
- **Docker Hub** – registry remoto per immagini Docker
- (Opzionale: Python, Node.js, ecc.)

## 🔄 Pipeline – Come funziona

1. Al push su `main`:
2. Il workflow si attiva (`.github/workflows/ci-cd.yml`)
3. Effettua il login su Docker Hub usando le GitHub Secrets
4. Costruisce l'immagine Docker
5. La pusha nel tuo repository Docker Hub

## 🔧 Come usarlo

1. Clona il repo
2. Modifica il codice dell'app se necessario
3. Effettua un commit su `main`
4. Guarda le Actions partire automaticamente da GitHub
