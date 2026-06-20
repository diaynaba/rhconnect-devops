# RHConnect — Infrastructure DevOps

> Plateforme SaaS de gestion des vacataires — ISM Dakar  
> Projet de fin d'études — Licence 3 GLRS & CDSD — 2025/2026  
> **Responsable DevOps : Diaynaba SOW**

## Architecture de déploiement
VM Ubuntu 24.04 (VirtualBox)

├── Nginx (reverse proxy) → :80

├── Spring Boot (backend) → :8080

├── Next.js (frontend) → :3000

├── PostgreSQL → :5432

├── Prometheus → :9090

├── Grafana → :3001

└── Jenkins (CI/CD) → :8081

## Stack technique

| Outil | Usage |
|---|---|
| Docker + Docker Compose | Conteneurisation de tous les services |
| Nginx | Reverse proxy + routage |
| PostgreSQL 15 | Base de données relationnelle |
| Spring Boot 3.x | Backend API REST |
| Next.js 16 | Frontend React |
| Prometheus | Collecte des métriques |
| Grafana | Visualisation des métriques |
| Jenkins | CI/CD pipeline |

## Lancer le projet

```bash
# Cloner le dépôt
git clone https://github.com/diaynaba/rhconnect-devops.git
cd rhconnect-devops

# Configurer les variables
cp .env.example .env
# Éditer .env avec vos valeurs

# Lancer tous les services
docker-compose up -d

# Vérifier
docker-compose ps
```

## Services accessibles

| Service | URL |
|---|---|
| Application | http://localhost/login |
| API Backend | http://localhost/api |
| Grafana | http://localhost:3001 |
| Prometheus | http://localhost:9090 |
| Jenkins | http://localhost:8081 |

## Responsable

**Diaynaba SOW** — Developer Full Stack & DevOps  
Module : Dashboard, KPIs, Notifications, Infrastructure  
Encadreur : M. Birane B. WANE — ISM Dakar
