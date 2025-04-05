# 🎨 ComicCrafter AI

ComicCrafter AI is a Flask-based web application that lets users generate 4-panel comic strips from a simple text prompt using Hugging Face and Stability AI APIs. It generates both the comic **storyline** and matching **cartoon-style images** for each panel. Users can then download the final 4-panel comic.

---

## 🚀 Problem Statement

Creating comics usually requires artistic skill and a good storyline. ComicCrafter AI solves this by letting anyone generate fun comic panels instantly with AI—no drawing or writing required.

---

## 🧠 Key Features

- ✅ Prompt-based story + image generation (4 panels)
- ✍️ Falcon-7B (Hugging Face) for comic storytelling
- 🎨 Stable Diffusion XL (Stability AI) for image generation
- 📥 One-click download for full comic
- 🖼 Cartoonish and light-hearted art style

---


📄 File Responsibilities
File / Folder	Purpose
app.py	Flask server: handles API, routes, calls AI models, processes output
templates/index.html	Webpage where user enters prompt and views comic
static/	Stores generated comic strips as PNGs (auto-created on generation)
requirements.txt	Python dependencies for easy setup
.gitignore	Prevents committing large or unnecessary files
README.md	Documentation file


## 🏗️ System Architecture Overview

```text
User Prompt
    │
    ▼
[Frontend (HTML + JS)]
    │
    ▼
[Flask Backend (app.py)]
    ├── Story Generation (Falcon-7B via Hugging Face API)
    ├── Image Generation (SDXL via Stability AI API)
    ▼
Final Render (HTML View + Download Panel Image)


