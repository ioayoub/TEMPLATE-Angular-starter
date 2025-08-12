# Angular 20 Template

Un template moderne et prêt à l’emploi pour démarrer rapidement des projets Angular 20 avec une intégration complète d’outils pour un workflow efficace et une qualité de code optimale.

## 🚀 Fonctionnalités principales

- **Angular 20** avec TypeScript strict
- **Tailwind CSS** configuré pour un style utilitaire rapide
- **Prettier** pour un formatage de code cohérent
- **Angular ESLint** pour le linting du code
- **Husky + lint-staged** pour automatiser les vérifications avant commit
- **GitHub Actions** pour lint, tests et vérification TypeScript en CI
- Génération de composants Angular avec **inline styles** (pas de fichiers CSS)


---

## 📦 Installation

1. **Cloner le projet ou l’utiliser comme template GitHub**
   
   ```
   git clone git@github.com:ioayoub/TEMPLATE-Angular-starter
   ```
   
   ```
   cd TEMPLATE-Angular-starter**
   ```


2. **Installer les dépendances**
  ```
  npm install

  ```

3. **Lancer le projet**
  ```
  ng serve
  ```
→ accessible par défaut sur [http://localhost:4200/](http://localhost:4200/)

---

## 🛠 Scripts disponibles

| Commande             | Description |
|----------------------|-------------|
| `npm start`          | Lance le serveur Angular (dev) |
| `npm test`           | Lance les tests unitaires |
| `npm run lint`       | Exécute Angular ESLint (ng lint) |
| `npm run prepare`    | Initialise Husky pour les hooks Git |

---

## 🎨 Tailwind CSS

- Fichier de config : `tailwind.config.js`
- Les classes sont disponibles dans tout le projet (`src/styles.css`).
- Configuration optimisée pour framework Angular.
- Création de composants Angular avec `inlineStyle: true` pour ne pas générer de fichiers CSS/SCSS.

---

## 🔍 Qualité du code

**Avant chaque commit** grâce à Husky :
- Lancement des tests (`npm test`)
- Vérification des types TypeScript (`tsc --noEmit`)
- Lint avec Angular ESLint (`ng lint`)
- Formatage des fichiers modifiés avec Prettier (`lint-staged`)

---

## ⚙ Intégration continue (CI)

Le fichier `.github/workflows/ci.yml` configure un pipeline GitHub Actions qui :
1. Installe les dépendances
2. Vérifie le typage TypeScript (`tsc --noEmit`)
3. Lance le lint (`ng lint`)
4. Exécute les tests Angular en **ChromeHeadless**

---

## 📄 Bonnes pratiques

- Respecter le format Prettier pour éviter les conflits
- Mettre à jour régulièrement Angular et Tailwind
- Ajouter d’autres hooks Git Husky si besoin (`pre-push`, `post-merge`, etc.)
- Adapter `angular.json`, `tsconfig.json` et `tailwind.config.js` aux besoins spécifiques

---

## 📌 Licence

Libre d’utilisation et de modification pour tout type de projet.

---


