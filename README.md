# Personal Website

This repository contains the source code of my personal website built with **[Hugo](https://gohugo.io/)**.  
It serves both as a personal project and as a showcase for static site deployment and CI/CD practices (via GitHub Actions).

---

## 🚀 Run locally with Hugo

1. Install Hugo (extended version recommended):  
   👉 [Installation guide](https://gohugo.io/getting-started/installing/)

2. Start the local server in the project root:
```bash
hugo server -D
```

Explanation:
- `-D` – includes content marked as **draft** in the preview  
- By default, the server runs at **http://localhost:1313**

3. Hugo automatically reloads the browser when you make changes.

---

## 📦 Build production version

To generate a static version of the site:
```bash
hugo
```

The static files will be created in the **`public/`** directory.  
Only the contents of this folder need to be published.

## ⚙️ Deployment with GitHub Actions

This project is configured to automatically build and deploy the site using **GitHub Actions**:

- The source code lives in the **`main`** branch.  
- On every push to `main`, GitHub Actions automatically:
  1. Runs Hugo to build the website.
  2. Publishes the generated static files to GitHub Pages.  

This setup not only keeps deployment simple but also demonstrates practical CI/CD automation.

## 📝 Project structure

- Main configuration → `config.toml` (or `config.yaml`)
- Content files → `content/`
- Theme files → `themes/`
- Static assets (images, CSS, JS) → `static/`

## 📚 Useful links

- [Hugo documentation](https://gohugo.io/documentation/)
- [GitHub Pages setup](https://docs.github.com/pages)

