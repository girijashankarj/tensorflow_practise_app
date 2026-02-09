<p align="center">
  <h1 align="center">tensorflow_practise_app</h1>
  <p align="center">
    A TensorFlow.js tutorial app that trains a linear regression model in the browser to predict MPG from car horsepower — with interactive visualizations.
  </p>
</p>

<p align="center">
  <a href="https://github.com/girijashankarj/tensorflow_practise_app"><img src="https://img.shields.io/github/last-commit/girijashankarj/tensorflow_practise_app?style=flat-square&logo=github" alt="last commit" /></a>
  <img src="https://img.shields.io/badge/TensorFlow.js-1.0-FF6F00?style=flat-square&logo=tensorflow&logoColor=white" alt="TensorFlow.js" />
  <img src="https://img.shields.io/badge/JavaScript-vanilla-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Type-Educational-FF9800?style=flat-square" alt="Educational" />
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat-square" alt="PRs welcome" />
</p>

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Quick Start](#quick-start)
- [How It Works](#how-it-works)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

**tensorflow_practise_app** is an educational project that demonstrates machine learning in the browser using TensorFlow.js. It fetches car data from an API, trains a neural network to learn the relationship between horsepower and MPG (miles per gallon), and visualizes both the training process and predictions — all in a single HTML file.

---

## Features

- **In-browser ML** — no server-side computation required
- **Data fetching** — loads car data from Google Cloud Storage API
- **Data cleaning** — filters and normalizes raw data
- **Scatter plot** — interactive Horsepower vs MPG visualization
- **Neural network** — sequential model with dense layers
- **Training visualization** — real-time loss/metrics charts
- **Predictions** — model predictions overlaid on original data
- **Min-max normalization** — proper data scaling

---

## Tech Stack

|                  | Details                              |
| ---------------- | ------------------------------------ |
| **ML Library**   | TensorFlow.js v1.0 (CDN)            |
| **Visualization**| TensorFlow.js Vis v1.0 (CDN)        |
| **Language**      | Vanilla JavaScript                   |
| **Data Source**   | Google Cloud Storage JSON API        |
| **Build Tool**   | None — runs directly in browser      |

---

## Quick Start

```bash
git clone https://github.com/girijashankarj/tensorflow_practise_app.git
cd tensorflow_practise_app
```

Open `index.html` directly in your browser — no build step required.

> The app fetches data from an external API, so an internet connection is needed.

---

## How It Works

```mermaid
flowchart LR
    A[Fetch car data<br/>from API] --> B[Clean & filter<br/>data]
    B --> C[Visualize<br/>scatter plot]
    C --> D[Create neural<br/>network model]
    D --> E[Train model<br/>with visualization]
    E --> F[Generate<br/>predictions]
    F --> G[Compare predictions<br/>vs original data]

    style A fill:#2196F3,color:#fff
    style D fill:#FF6F00,color:#fff
    style G fill:#4CAF50,color:#fff
```

| Step                  | Description                                           |
| --------------------- | ----------------------------------------------------- |
| **Data loading**      | Fetches car dataset from Google Cloud Storage         |
| **Data cleaning**     | Filters out entries with missing horsepower/MPG       |
| **Visualization**     | Renders scatter plot using tfjs-vis                   |
| **Model creation**    | Sequential model with dense layers (input → hidden → output) |
| **Training**          | Trains with loss visualization using `model.fit()`    |
| **Prediction**        | Generates predictions and compares to original data   |
| **Normalization**     | Min-max scaling for input/output tensors              |

---

## Project Structure

```
tensorflow_practise_app/
├── index.html          # Main HTML file (CDN imports for TF.js)
├── script.js           # Complete ML pipeline implementation
└── README.md
```

---

## Contributing

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/my-feature`
3. **Make** your changes
4. **Commit** and open a Pull Request

---

## License

This project is open source. See the [LICENSE](LICENSE) file for details.

---

<p align="center">
  Built with discipline by <a href="https://github.com/girijashankarj">GarryTJ</a>
</p>
