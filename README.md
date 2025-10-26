# ☕ The Daily Grind

> Un site web élégant et chaleureux pour café artisanal, construit avec Astro et Tailwind CSS v4.

![Astro](https://img.shields.io/badge/Astro-FF5D01?style=for-the-badge&logo=astro&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)

---

## 📋 Table des Matières

- [À Propos](#-à-propos)
- [Démarrage Rapide](#-démarrage-rapide)
- [Structure du Projet](#-structure-du-projet)
- [Palette de Couleurs](#-palette-de-couleurs)
- [Technologies Utilisées](#-technologies-utilisées)
- [Scripts Disponibles](#-scripts-disponibles)
- [Comment Contribuer](#-comment-contribuer)
- [Bonnes Pratiques](#-bonnes-pratiques)

---

## 🎯 À Propos

**The Daily Grind** est un site web moderne pour café artisanal présentant :
- 🎨 Design terreux et chaleureux inspiré du monde du café
- 🌊 Transitions SVG ondulées élégantes
- 📱 Interface entièrement responsive
- 🎠 Carousel de menu interactif
- 🇫🇷 Contenu en français

---

## 🚀 Démarrage Rapide

### Prérequis

- **Node.js** : v18.0.0 ou supérieur
- **pnpm** : Gestionnaire de paquets recommandé

### Installation

```bash
# Cloner le repository
git clone https://github.com/Newneri/TheDailyGrind.git

# Naviguer dans le dossier
cd TheDailyGrind

# Installer les dépendances
pnpm install

# Lancer le serveur de développement
pnpm dev
```

Le site sera accessible sur `http://localhost:4321` 🎉

---

## 📁 Structure du Projet

```
TheDailyGrind/
├── public/              # Fichiers statiques (favicon, logo)
├── src/
│   ├── assets/          # Images et ressources
│   │   └── images/
│   │       └── drinks/  # Photos des boissons
│   ├── components/      # Composants Astro
│   │   ├── Header.astro    # Navigation principale
│   │   ├── Hero.astro      # Section héro avec transitions
│   │   └── Menu.astro      # Carousel de menu
│   ├── layouts/
│   │   └── Layout.astro    # Layout principal
│   ├── pages/
│   │   └── index.astro     # Page d'accueil
│   └── styles/
│       └── global.css      # Styles globaux et configuration Tailwind
├── astro.config.mjs     # Configuration Astro
├── package.json
└── tsconfig.json
```

---

## 🎨 Palette de Couleurs

Notre palette évoque la chaleur et l'authenticité d'un café artisanal :

### Couleurs Principales

| Couleur | Hex | Usage | Aperçu |
|---------|-----|-------|--------|
| **Dark Coffee** | `#4A3C32` | Texte principal, navigation | 🟤 |
| **Warm Cream** | `#F5F2EC` | Arrière-plans clairs | ⚪ |

### Couleurs Secondaires

| Couleur | Hex | Usage | Aperçu |
|---------|-----|-------|--------|
| **Toasted Almond** | `#C2B2A2` | Arrière-plans secondaires, bordures | 🟫 |
| **Deep Forest Green** | `#5D6D5F` | Accents, liens, icônes | 🟢 |

### Couleurs d'Accent

| Couleur | Hex | Usage | Aperçu |
|---------|-----|-------|--------|
| **Burnt Orange** | `#CC7A46` | Boutons CTA, highlights | 🟠 |
| **Soft Gold** | `#D4A373` | Éléments décoratifs premium | 🟡 |

### Couleurs Utilitaires

| Couleur | Hex | Usage | Aperçu |
|---------|-----|-------|--------|
| **Off-Black** | `#2C2C2C` | Texte sur fonds clairs | ⚫ |
| **Light Gray** | `#E0DCD7` | Bordures subtiles, dividers | ⚪ |
| **Pure White** | `#FFFFFF` | Contraste élevé | ⚪ |

### Utilisation dans le Code

```astro
<!-- Classes Tailwind avec couleurs personnalisées -->
<div class="bg-warm-cream text-dark-coffee">
  <button class="bg-burnt-orange hover:bg-dark-coffee text-pure-white">
    Commander
  </button>
</div>
```

---

## 🛠 Technologies Utilisées

- **[Astro](https://astro.build/)** - Framework web moderne et ultra-rapide
- **[Tailwind CSS v4](https://tailwindcss.com/)** - Framework CSS utility-first
- **[TypeScript](https://www.typescriptlang.org/)** - JavaScript typé
- **[pnpm](https://pnpm.io/)** - Gestionnaire de paquets rapide et efficace

---

## 📜 Scripts Disponibles

```bash
# Développement - Lance le serveur avec hot reload
pnpm astro dev

# Build - Compile le site pour la production
pnpm astro build

# Preview - Prévisualise le build de production
pnpm astro preview

# Astro CLI - Accède aux commandes Astro
pnpm astro
```

---

## 🤝 Comment Contribuer

Nous accueillons les contributions ! Voici comment participer :

### 1. Fork & Clone

```bash
# Fork le projet sur GitHub puis clone ton fork
git clone https://github.com/TON-USERNAME/TheDailyGrind.git
cd TheDailyGrind
```

### 2. Créer une Branche

```bash
# Créer une branche pour ta fonctionnalité
git checkout -b feature/ma-nouvelle-fonctionnalite

# Ou pour un bug fix
git checkout -b fix/correction-bug
```

### 3. Développer

```bash
# Installer les dépendances
pnpm install

# Lancer le serveur de dev
pnpm dev

# Faire tes modifications...
```

### 4. Commit & Push

```bash
# Ajouter tes changements
git add .

# Commit avec un message clair
git commit -m "✨ Ajout: nouvelle section blog"

# Push vers ton fork
git push origin feature/ma-nouvelle-fonctionnalite
```

### 5. Pull Request

Ouvre une Pull Request sur le repo principal avec :
- 📝 Description claire des changements
- 🖼️ Screenshots si modifications visuelles
- ✅ Tests effectués

---

## ✨ Bonnes Pratiques

### Code Style

- **Composants** : Utiliser des composants Astro (`.astro`) pour les éléments réutilisables
- **Tailwind** : Privilégier les classes utilitaires, éviter le CSS custom
- **Responsive** : Mobile-first approach avec les breakpoints `sm:`, `md:`, `lg:`, `xl:`
- **Accessibilité** : Toujours inclure des attributs `alt` sur les images

### Commits

Utiliser des préfixes clairs :
- `✨ Ajout:` - Nouvelle fonctionnalité
- `🐛 Fix:` - Correction de bug
- `💄 Style:` - Changements visuels
- `📝 Doc:` - Documentation
- `♻️ Refactor:` - Refactorisation de code
- `🚀 Perf:` - Amélioration de performance

### Structure des Fichiers

```
src/components/NouveauComposant.astro
```

```astro
---
// Imports et logique TypeScript
import type { Props } from './types';
---

<!-- Markup HTML -->
<section class="bg-warm-cream">
  <!-- Contenu -->
</section>

<style>
  /* Styles scopés si nécessaire */
</style>
```

---

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

---

## 💬 Contact & Support

- 🐛 **Issues** : [GitHub Issues](https://github.com/Newneri/TheDailyGrind/issues)
- 💡 **Discussions** : [GitHub Discussions](https://github.com/Newneri/TheDailyGrind/discussions)

---

<p align="center">
  Fait avec ❤️ et beaucoup de ☕
</p>