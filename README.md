# 🥐 Bakry Store - Artisanal Bakery Storefront

A modern, elegant, and interactive single-page application (SPA) for an artisanal bakery. This project demonstrates advanced state management with **Vuex**, component-based architecture, dynamic routing using **Vue Router**, and responsive styling.

---

## ✨ Features

- **🥐 Interactive Product Catalog**: Browse a delicious selection of freshly baked goods with detailed prices, categories, and ratings.
- **🔍 Dynamic Product Details**: Access detailed ingredient lists, preparation times, and descriptions for individual products.
- **🛒 Centralized Cart System**: 
  - Real-time cart calculations (subtotal, shipping, totals).
  - Modify item quantities directly from the cart drawer.
  - One-click checkout with toast confirmation.
- **⚙️ Product Management Dashboard**: 
  - Full CRUD operations (Add, Edit, Delete products).
  - Dynamic calculations for store statistics (average price, highest-rated product).
- **🔔 Toast Notification System**: Instant, automated feedback for user actions (adding items to the cart, modifying store products, and checking out).

---

## 🛠️ Tech Stack & Libraries

- **Framework**: [Vue 3](https://vuejs.org/) (Composition API & Options API styles)
- **State Management**: [Vuex 4](https://vuex.vuejs.org/)
- **Routing**: [Vue Router 4](https://router.vuejs.org/) (configured with hash history for production reliability)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/)
- **Build Tool**: [Vite](https://vite.dev/)
- **Deployment**: [GitHub Pages](https://pages.github.com/)

---

## 📁 Project Structure

```text
bakry-store/
├── public/                # Static assets (images, icons)
├── src/
│   ├── components/        # Reusable UI Components (Navbar, Footer, Card, etc.)
│   ├── pages/             # Page components (Home, About, Products, Product Details, Management)
│   ├── routes/            # Vue Router configuration
│   ├── store/             # Vuex centralized state management
│   ├── App.vue            # Main root component
│   ├── main.js            # App initialization and entry point
│   ├── style.css          # Tailwind/CSS styling imports
│   └── data.json          # Initial mock product data
├── vite.config.js         # Vite configuration (base URL set for GitHub Pages)
└── package.json           # Dependencies and build/deploy scripts
```

---

## 🚀 Getting Started

### Prerequisites

Make sure you have Node.js and npm installed on your machine.

### Installation

1. Clone the repository and navigate to the project directory:
   ```sh
   cd VUE/D02/bakry-store
   ```

2. Install dependencies:
   ```sh
   npm install
   ```

3. Run the development server:
   ```sh
   npm run dev
   ```

4. Build the application for production:
   ```sh
   npm run build
   ```

---

## 🌐 Deployment to GitHub Pages

The project is fully pre-configured to build and deploy to GitHub Pages.

### Script Setup

The following scripts are added to `package.json`:
- `"predeploy": "npm run build"`: Pre-compiles the production bundle into the `dist` directory.
- `"deploy": "gh-pages -d dist"`: Pushes the compiled `dist` directory to the `gh-pages` branch.

### How to Deploy

To publish changes to GitHub Pages:
```sh
npm run deploy
```

> **Note**: Make sure to check the repository settings on GitHub (**Settings** > **Pages**) and set the source branch for build and deployment to **`gh-pages`**.
