# <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/moon.svg" width="24" height="24" alt="HelloLuna" /> HelloLuna - Automatisation de Gestion de Rendez-vous avec IA

<div align="center">

  <img src="https://img.shields.io/badge/Version-1.0.0-blue.svg" alt="Version" />
  <img src="https://img.shields.io/badge/License-Proprietary-red.svg" alt="License" />
  <img src="https://img.shields.io/badge/TypeScript-5.0-blue.svg" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Next.js-14-black.svg" alt="Next.js" />
  <img src="https://img.shields.io/badge/Node.js-18+-green.svg" alt="Node.js" />
  <img src="https://img.shields.io/badge/PostgreSQL-16-blue.svg" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/OpenAI-GPT--4-purple.svg" alt="OpenAI" />

</div>

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/clipboard-list.svg" width="20" height="20" alt="Description" /> Description

HelloLuna est une plateforme SaaS révolutionnaire qui automatise 90% de la gestion de rendez-vous pour les professionnels grâce à une IA conversationnelle intelligente. Conçue pour les coiffeurs, dentistes, jardiniers et tous les professionnels ayant besoin de gérer un agenda, HelloLuna transforme la gestion de rendez-vous en un processus automatisé et intelligent.

L'application utilise l'intelligence artificielle (OpenAI GPT-4) pour gérer les conversations avec les clients via WhatsApp, SMS et appels téléphoniques, permettant aux professionnels de se concentrer sur leur cœur de métier tout en offrant une expérience client exceptionnelle.

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/sparkles.svg" width="20" height="20" alt="Features" /> Fonctionnalités principales

### <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/bot.svg" width="18" height="18" alt="IA" /> IA Conversationnelle Intelligente

- **Multi-canal** : WhatsApp, SMS, Appels téléphoniques (Twilio)

- **Compréhension contextuelle** : L'IA comprend les besoins spécifiques de chaque client

- **Génération de réponses naturelles** : Conversations fluides et humaines

- **Function Calling** : L'IA peut directement interagir avec l'agenda (vérifier disponibilité, créer rendez-vous, etc.)

### <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/wrench.svg" width="18" height="18" alt="Service Builder" /> Service Builder Universel

- **Création flexible** : Configurez vos services avec tous les paramètres nécessaires

- **Banque de questions intelligente** : Système de questions pré-définies par type d'activité

- **Génération automatique par IA** : ChatGPT génère automatiquement 5 questions personnalisées pour chaque service

- **Drag & Drop intuitif** : Interface visuelle pour organiser les questions de conversation

- **Personnalisation complète** : Ajoutez vos propres questions personnalisées

### <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/calendar.svg" width="18" height="18" alt="Optimisation" /> Optimisation Intelligente des Créneaux

- **Maximisation du taux de remplissage** : L'algorithme optimise l'utilisation de votre agenda

- **Minimisation des temps morts** : Réduit les périodes d'inactivité

- **Optimisation des revenus** : Privilégie les créneaux les plus rentables

- **Équilibrage de charge** : Répartit intelligemment les rendez-vous entre praticiens

### <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/check-circle.svg" width="18" height="18" alt="Confirmations" /> Confirmations et Rappels Intelligents

- **Confirmations automatiques** : Envoi immédiat après réservation

- **Rappels programmés** : 24h et 2h avant le rendez-vous

- **Personnalisation des messages** : Adaptés à chaque client et service

- **Multi-canal** : WhatsApp, SMS, Email

### <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/users.svg" width="18" height="18" alt="Expérience Client" /> Expérience Client Post-Visite

- **Demande de feedback automatique** : Collecte d'avis après chaque rendez-vous

- **Système de fidélité** : Suivi des clients réguliers

- **Historique complet** : Toutes les interactions et préférences enregistrées

- **Profil client enrichi** : L'IA apprend des préférences pour personnaliser les futures interactions

### <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/bar-chart.svg" width="18" height="18" alt="Dashboard" /> Dashboard et Analytics

- **Vue d'ensemble en temps réel** : Rendez-vous du jour, semaine, mois

- **Métriques clés** : Taux de remplissage, revenus, nouveaux clients

- **Analytics avancés** : Tendances, prévisions, insights

- **Export de données** : Rapports personnalisables

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/network.svg" width="20" height="20" alt="Architecture" /> Architecture technique

| Composant | Technologie |
|-----------|-------------|
| **Frontend** | Next.js 14 + React 18 + TypeScript + Tailwind CSS + shadcn/ui |
| **Backend** | Node.js + Express + TypeScript + Prisma ORM |
| **Base de données** | PostgreSQL 16 |
| **IA** | OpenAI GPT-4 Turbo + Function Calling |
| **Communication** | Twilio (WhatsApp, SMS, Voice) |
| **Cache** | Redis (optionnel) |
| **Containerisation** | Docker + Docker Compose |

### Structure du projet

```
HelloLuna/
├── packages/
│   ├── backend/          # API REST Node.js + Express
│   │   ├── src/
│   │   │   ├── routes/   # Endpoints API
│   │   │   ├── services/ # Logique métier (IA, optimisation)
│   │   │   ├── middleware/# Auth, validation, erreurs
│   │   │   └── lib/      # Configuration (Prisma, etc.)
│   │   └── prisma/       # Schéma de base de données
│   │
│   └── frontend/         # Application Next.js 14
│       ├── app/          # Pages et routes
│       ├── components/   # Composants React réutilisables
│       └── lib/          # Utilitaires et API client
│
├── docker-compose.yml    # Services Docker (PostgreSQL, Redis)
└── package.json          # Configuration monorepo
```

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/rocket.svg" width="20" height="20" alt="Installation" /> Installation rapide

### Prérequis

- **Node.js** 18+ et npm

- **Docker** et Docker Compose

- **Git**

- **Clé API OpenAI** : [platform.openai.com](https://platform.openai.com)

- **Compte Twilio** (optionnel pour les communications) : [twilio.com](https://www.twilio.com)

### Installation

#### 1. Cloner le repository

```bash
git clone https://github.com/OliverThys/HelloLuna.git
cd HelloLuna
```

#### 2. Installer les dépendances

```bash
npm install
```

#### 3. Configurer l'environnement

Créez les fichiers de configuration :

**`packages/backend/config.local.env`** :
```env
DATABASE_URL="postgresql://user:password@localhost:5432/helloluna?schema=public"
OPENAI_API_KEY="sk-your-openai-api-key"
JWT_SECRET="your-secret-jwt-key"
JWT_REFRESH_SECRET="your-secret-refresh-key"
TWILIO_ACCOUNT_SID="your-twilio-account-sid"
TWILIO_AUTH_TOKEN="your-twilio-auth-token"
TWILIO_PHONE_NUMBER="+1234567890"
```

**`packages/frontend/.env.local`** :
```env
NEXT_PUBLIC_API_URL=http://127.0.0.1:3001
```

#### 4. Démarrer les services Docker

```bash
docker-compose up -d
```

#### 5. Initialiser la base de données

```bash
cd packages/backend
npx prisma db push
npm run db:seed
```

#### 6. Démarrer l'application

Depuis la racine :
```bash
npm run dev
```

Ou séparément :
```bash
# Terminal 1 - Backend
cd packages/backend
npm run dev

# Terminal 2 - Frontend
cd packages/frontend
npm run dev
```

#### 7. Accéder à l'application

| Service | URL | Description |
|---------|-----|-------------|
| **Frontend** | http://127.0.0.1:3000 | Interface utilisateur |
| **Backend API** | http://127.0.0.1:3001 | API REST |
| **PostgreSQL** | localhost:5432 | Base de données |

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/smartphone.svg" width="20" height="20" alt="Usage" /> Utilisation

### Connexion

Créez un compte via la page d'inscription ou connectez-vous avec vos identifiants.

### Workflow principal

1. **Configuration de l'organisation** : Définissez le type d'activité de votre entreprise

2. **Création de services** : Configurez vos services avec durée, prix, description

3. **Gestion des questions** : Utilisez la banque de questions ou générez-en avec l'IA

4. **Optimisation des créneaux** : L'algorithme suggère les meilleurs horaires

5. **Suivi des rendez-vous** : Consultez votre dashboard en temps réel

6. **Interactions automatisées** : L'IA gère les conversations avec vos clients

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/shield-check.svg" width="20" height="20" alt="Security" /> Sécurité et conformité

- **Authentification JWT** : Tokens avec expiration + refresh tokens

- **Isolation multi-tenant** : Isolation complète des données au niveau base de données

- **Rate limiting** : Protection contre les abus sur toutes les routes

- **Validation Zod** : Validation stricte de tous les inputs

- **Helmet.js** : Sécurité HTTP renforcée

- **Conformité RGPD** : Chiffrement, pseudonymisation, droits utilisateurs (accès, oblivion, rectification, portability, opposition)

- **Audit log** : Enregistrement de toutes les actions sensibles

- **RBAC** : Gestion des rôles et permissions

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/wrench.svg" width="20" height="20" alt="Development" /> Développement

### Backend

```bash
cd packages/backend

# Développement
npm run dev

# Build
npm run build

# Base de données
npm run db:generate  # Générer le client Prisma
npm run db:migrate   # Exécuter les migrations
npm run db:seed      # Seed la base de données
```

### Frontend

```bash
cd packages/frontend

# Développement
npm run dev

# Build production
npm run build

# Démarrer en production
npm run start
```

### Scripts monorepo

```bash
# Depuis la racine
npm run dev    # Démarrer backend + frontend
npm run build  # Build complet
npm run lint   # Linting
```

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/flask-conical.svg" width="20" height="20" alt="Tests" /> Tests

```bash
# Backend
cd packages/backend
npm test

# Frontend
cd packages/frontend
npm test

# Tests E2E
npm run test:e2e
```

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/package.svg" width="20" height="20" alt="Deployment" /> Déploiement production

### Build

```bash
# Build complet
npm run build

# Build backend uniquement
cd packages/backend
npm run build

# Build frontend uniquement
cd packages/frontend
npm run build
```

### Variables d'environnement production

Assurez-vous de configurer toutes les variables d'environnement nécessaires pour la production :

- `DATABASE_URL` : URL de la base de données PostgreSQL

- `OPENAI_API_KEY` : Clé API OpenAI

- `JWT_SECRET` et `JWT_REFRESH_SECRET` : Secrets JWT sécurisés

- `TWILIO_*` : Identifiants Twilio pour les communications

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/bar-chart.svg" width="20" height="20" alt="Monitoring" /> Monitoring

Le dashboard intégré permet de suivre :

- **Statistiques en temps réel** : Rendez-vous du jour, semaine, mois

- **Métriques de performance** : Taux de remplissage, revenus

- **Analytics** : Tendances et prévisions

- **Alertes** : Notifications importantes

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/book-open.svg" width="20" height="20" alt="Documentation" /> Documentation

### Base de données

Le schéma Prisma inclut 13 modèles principaux :

- **Organization** : Organisations multi-tenant

- **Member** : Membres de l'organisation

- **Service** : Services proposés

- **QuestionTemplate** : Banque de questions

- **Customer** : Clients avec historique

- **Appointment** : Rendez-vous

- **Practitioner** : Praticiens

- **Availability** : Horaires de disponibilité

- **Conversation** & **Message** : Historique des conversations IA

- **Notification** : Rappels et confirmations

- **Feedback** : Avis clients

### API

L'API REST est accessible sur `http://127.0.0.1:3001/api` avec les endpoints suivants :

- `/api/auth/*` : Authentification

- `/api/services/*` : Gestion des services

- `/api/questions/*` : Banque de questions

- `/api/customers/*` : Gestion des clients

- `/api/appointments/*` : Gestion des rendez-vous

- `/api/ai/*` : Interactions IA

- `/api/twilio/*` : Webhooks Twilio

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/git-branch.svg" width="20" height="20" alt="Roadmap" /> Roadmap

### Phase 1 : MVP <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/check-circle.svg" width="16" height="16" alt="Terminé" />

- [x] Architecture de base

- [x] Authentification et gestion d'organisations

- [x] Service Builder avec banque de questions

- [x] Génération automatique de questions par IA

- [x] Interface drag & drop pour gestion des questions

- [x] Système de base de données complet

### Phase 2 : IA Conversationnelle <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/construction.svg" width="16" height="16" alt="En cours" />

- [ ] Intégration complète OpenAI avec function calling

- [ ] Support multi-canal (WhatsApp, SMS, Voice)

- [ ] Gestion des conversations et historique

- [ ] Optimisation intelligente des créneaux

### Phase 3 : Automatisation <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/calendar.svg" width="16" height="16" alt="Automatisation" />

- [ ] Système de confirmations automatiques

- [ ] Rappels programmés (24h, 2h avant)

- [ ] Gestion des disponibilités

- [ ] Blocage de créneaux

### Phase 4 : Analytics et Optimisation <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/bar-chart.svg" width="16" height="16" alt="Analytics" />

- [ ] Dashboard complet avec métriques

- [ ] Analytics avancés

- [ ] Rapports exportables

- [ ] A/B testing des stratégies de réservation

### Phase 5 : Expérience Client <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/users.svg" width="16" height="16" alt="Client" />

- [ ] Système de feedback post-visite

- [ ] Programme de fidélité

- [ ] Profils clients enrichis

- [ ] Recommandations personnalisées

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/users.svg" width="20" height="20" alt="Contributing" /> Contribution

Les contributions sont les bienvenues ! Pour contribuer :

1. Fork le projet

2. Créez votre branche (`git checkout -b feature/AmazingFeature`)

3. Commit vos changements (`git commit -m 'Add some AmazingFeature'`)

4. Push vers la branche (`git push origin feature/AmazingFeature`)

5. Ouvrez une Pull Request

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/file-text.svg" width="20" height="20" alt="License" /> Licence

**Copyright © 2025 HelloLuna. Tous droits réservés.**

Ce projet est sous licence propriétaire.

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/help-circle.svg" width="20" height="20" alt="Support" /> Support

| Ressource | Lien |
|-----------|------|
| **Repository GitHub** | [https://github.com/OliverThys/HelloLuna](https://github.com/OliverThys/HelloLuna) |
| **Issues GitHub** | [https://github.com/OliverThys/HelloLuna/issues](https://github.com/OliverThys/HelloLuna/issues) |

---

## <img src="https://raw.githubusercontent.com/lucide-icons/lucide/main/icons/heart.svg" width="20" height="20" alt="Acknowledgments" /> Remerciements

- Communauté open source (Next.js, React, Prisma, OpenAI)

- Contributeurs et développeurs du projet

- Utilisateurs pour leurs retours et suggestions

---

<div align="center">

  <strong>HelloLuna</strong> - Automatisez votre agenda, concentrez-vous sur votre métier

</div>

