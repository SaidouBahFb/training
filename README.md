Ce projet est un exemple complet pour apprendre le DevOps en utilisant :

Backend : Node.js + Express + MySQL

Frontend : React (servi avec Nginx)

Infra : Docker, Docker Compose

(bientôt) CI/CD avec GitHub Actions et déploiement sur Minikube/Kubernetes

devops-projet/
backend/ # API Node.js (Express + MySQL)
frontend/ # Application React
infra/ # Docker Compose + MySQL init
.github/
workflows/ # CI/CD pipelines

Lancer avec Docker Compose :
docker compose up -d --build

Un workflow GitHub Actions construit et pousse automatiquement les images Docker :

training-backend:latest

training-frontend:latest

sur Docker Hub

Auteur

Projet créé par Saidou Bah pour apprendre et pratiquer le DevOps.
