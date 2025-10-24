# 🎬 Optifit

## 👋 Introduction

Je m’appelle **Gabriel**, je suis apprenti développeur chez **socraft SA**, une entreprise spécialisée dans le développement de solutions logicielles sur mesure et dans l’accompagnement de startups.

Aujourd’hui, je vais vous présenter le **système de qualité** est en place chez **Optifit**, une application de gestion de tournois et de compétitions sportives que j’ai créée en **2022**.

Tout a commencé quand j’étais encore à **l’école obligatoire**.  
À l’époque, je participais à de petits tournois de sport à l'école, et j’ai remarqué que tout était encore géré sur papier ou dans des fichiers Excel.  
Et sachant coder, je me suis dit qu'on pouvait sûrement faire mieux.
J’ai donc développé un premier **Proof of Concept (POC)** que j’ai présenté à mes professeurs d’éducation physique.  
Ce projet scolaire est devenu, trois ans plus tard, une **application professionnelle** utilisée à grande échelle.

Aujourd’hui, Optifit est utilisée par **une cinquantaine d'associations sportives** en Suisse romande, notamment par l’**ACVF** pour le tournoi *Graines de Foot*, qui réunit chaque année plus de **10’000 jeunes joueurs et joueuses**.

Depuis septembre 2025, nous sommes **quatre** à travailler sur le projet :

- **Gabriel** – CTO, Tech lead, coordination  
- **Dmytro** – branding et expérience utilisateur  
- **José** et **Thomas** – aident pour le développement frontend et backend
- **socraft SA** nous accompagne sur la stratégie, le développement de la startup

---

## 🧠 Stack technique

- **Frontend :** React, TypeScript, Vite, Tailwind, Shadcn, Vitest  
- **Backend :** NestJS, TypeScript, Jest, Socket.io  
- **Déploiement :** Firebase Hosting (frontend) + Cloud Run (backend Docker)  
- **CI/CD :** GitHub Actions
- **Services externes :**
  - Auth0 comme IDP provider
  - Firestore et Cloud Storage (Bases de donnés)
  - Stripe pour les paiements
  - SMTP2GO pour l'envoi de mails

---

## ✅ Système de qualité

### 🧩 Philosophie

> Tolérance zéro pour le code non testé ou non compréhensible.  
> Chaque ligne de code doit être claire, documentée et vérifiée.

### 🔬 Types de tests

- **Backend :**
  - Tests unitaires et d’intégration (Jest)
  - Couverture de **85–90%**
  - Lancement automatique à chaque commit
- **Frontend :**
  - Tests unitaires ciblés (Vitest)
  - Tests manuels systématiques en QA
- **Tests de charge :**
  - Réalisés ponctuellement avant les grands événements (ex : Graines de Foot)

### 🧰 Outils utilisés

- **ESLint / Prettier** – cohérence du code  
- **GitHub Actions** – CI/CD, tests, lint, build  
- **Sentry** – alerting d’erreurs en production  
- **PostHog** – analytics et comportement utilisateur  
- **Notion** – documentation technique et procédures  
- **Trello** – gestion des tâches et priorités

### 🌍 Environnements

- **Local :** développement individuel avec base de tests  
- **QA :** déploiement automatique à chaque Pull Request  
- **Production :** déploiement automatisé après validation sur `main`

---

## ⚙️ Intégration du système qualité dans le développement

### 🔁 Processus

1. Création d’une **branche dédiée** à une nouvelle fonctionnalité  
2. Développement + **ajout des tests nécessaires**  
3. **Push** sur GitHub → GitHub Actions exécute tests, lint et build  
4. **Déploiement automatique en QA** avec sandbox Stripe/Auth0  
5. Relecture du code + tests manuels par un autre membre de l’équipe  
6. Validation → **merge sur `main`** → déploiement automatique en **production**

### 👥 Rôles dans l’équipe

- **Gabriel** – lead technique, validation finale, architecture  
- **Dmytro** – cohérence visuelle et UX  
- **José & Thomas** – développement et relecture mutuelle  
- **socraft** – Nous accompagnent également sur la qualité de notre application

### ⚡ Automatisations clés

- **GitHub Actions** : tests, build, lint, déploiement QA/Prod  
- **Sentry** : alertes temps réel  
- **PostHog** : suivi et analytics  
- **Google Cloud** : Fait tourner notre app, backups hebdomadaires de nos bases de données

### 💬 Culture d’équipe

> Si un code n’est pas clair, on le réécrit.  
> Si un comportement n’est pas testé, on ne merge pas.  
> Si une erreur survient, on est alerté immédiatement.

---

## 🏁 Conclusion

Optifit est né d’un simple **POC d’écolier**, et est aujourd’hui une **solution complète et fiable** utilisée à grande échelle.  
Si le projet a pu évoluer aussi vite, c’est grâce à un **système de qualité solide**, intégré à chaque étape du développement.

Chez nous, la qualité n’est pas une étape finale :  
c’est une **culture**, un **réflexe** et une **garantie** de confiance pour nos utilisateurs.

**Merci.**
