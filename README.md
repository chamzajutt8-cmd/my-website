<div align="center">

# 🌐 My Website

### A sleek, static product showcase — containerized and deployed with a full CI/CD pipeline.

[![Docker](https://img.shields.io/badge/Docker-ready-2496ED?logo=docker&logoColor=white)](https://hub.docker.com/)
[![CI/CD](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)](.github/workflows)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](#)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](#)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](#-license)

</div>

---

## ✨ Overview

**My Website** is a lightweight, static front-end project that showcases a dynamic product listing (built with vanilla HTML, CSS, and JavaScript) — no frameworks, no build tools, just clean fundamentals. The project is fully containerized with **Docker** and ships through an automated **GitHub Actions** pipeline straight to **Docker Hub**, making it easy to build, ship, and run anywhere.

## 🚀 Features

- 🛍️ **Dynamic product rendering** — products are defined in a JS array and rendered to the page on load
- 🎨 **Clean, responsive styling** with plain CSS — no dependencies
- 🐳 **Dockerized** — consistent environment from local dev to production
- ⚙️ **Automated CI/CD** — every push builds and publishes a Docker image via GitHub Actions
- 🔒 **Secrets-based deployment** — Docker Hub credentials handled securely via repository secrets
- 📦 **Zero build step** — pure HTML/CSS/JS, runs anywhere a browser or web server does

## 🗂️ Project Structure

```
my-website/
├── .github/
│   └── workflows/       # CI/CD pipeline (build & push to Docker Hub)
├── Dockerfile           # Container build definition
├── index.html           # Main page + product data/rendering logic
└── style.css            # Styling
```

## 🛠️ Tech Stack

| Layer            | Technology            |
|-------------------|------------------------|
| Markup            | HTML5                 |
| Styling           | CSS3                  |
| Interactivity     | Vanilla JavaScript    |
| Containerization  | Docker                |
| CI/CD             | GitHub Actions        |
| Registry          | Docker Hub            |

## 📦 Getting Started

### Option 1 — Just open it
Since this is a static site, you can simply open it in your browser:

```bash
git clone https://github.com/chamzajutt8-cmd/my-website.git
cd my-website
open index.html   # or double-click the file
```

### Option 2 — Run with Docker

```bash
# Build the image
docker build -t my-website .

# Run the container
docker run -d -p 8080:80 my-website
```

Then visit **http://localhost:8080** in your browser.

> ℹ️ Adjust the exposed port above (`80`) if your `Dockerfile` serves on a different port.

## ⚙️ CI/CD Pipeline

Every push to the repository triggers a GitHub Actions workflow that:

1. Checks out the latest code
2. Builds the Docker image
3. Logs in to Docker Hub using repository secrets
4. Pushes the newly built image to Docker Hub

This means the containerized version of the site is always in sync with the latest commit — no manual deployment steps required.

## 🖼️ Preview

<div align="center">
  <sub>Add a screenshot or GIF of the site here for maximum impact ✨</sub>
</div>

```md
![Website Preview](./assets/preview.png)
```

## 🧭 Roadmap

- [ ] Add more product categories
- [ ] Improve mobile responsiveness
- [ ] Add a live GitHub Pages / hosted demo link
- [ ] Write unit tests for JS logic

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!
Feel free to check the [issues page](../../issues) or open a pull request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the **MIT License** — feel free to use, modify, and share.

## 👤 Author

**Hamza Jutt**
GitHub: [@chamzajutt8-cmd](https://github.com/chamzajutt8-cmd)

---

<div align="center">
  <sub>Built with ❤️ and a lot of curly braces.</sub>
</div>
