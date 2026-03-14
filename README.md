# 🧬 Interactive 3D DNA Structural Simulator

[![GitHub Pages](https://img.shields.io/badge/Hosted_on-GitHub_Pages-blue?logo=github)](https://<your-username>.github.io/<your-repo-name>/)
[![Made with Three.js](https://img.shields.io/badge/Made_with-Three.js-red?logo=three.js)](https://threejs.org/)

**[👉 View the Live 3D Simulation Here](https://aishwarya-926.github.io/dna-model/)**

*(Note: Replace the links above with your actual GitHub username and repository name)*

## 📖 Overview
This project is an interactive, browser-based 3D educational tool designed to answer the prompt: *"Prepare a model for the A, B, or Z forms of deoxyribonucleic acid."* 

Instead of a static physical model, this project leverages the power of WebGL and **Three.js** to dynamically generate highly accurate 3D structural models of the three primary conformations of DNA: **A-DNA**, **B-DNA**, and **Z-DNA**. 

**🔥 Latest Feature Update:** The model now includes a live API fetch to the **RCSB Protein Data Bank** for a high-definition NMR structure of B-DNA. It dynamically filters out structural water molecules and utilizes high-performance distance-squared mathematics to calculate and render a flawless, fully-bonded Ball-and-Stick chemical model—including all Hydrogen atoms!

## ✨ Features
* **Real-Time 3D Rendering:** Fully interactive molecule. You can rotate, pan, and zoom to inspect the molecular structure from any angle.
* **Toggle Auto-Rotation:** Users can pause and resume the automatic spinning of the structure for closer inspection.
* **Abstract Conformation Mode:** Procedurally generated geometry comparing the structural statistics of:
  * **B-DNA:** The standard, right-handed Watson-Crick double helix.
  * **A-DNA:** The compressed, wider, right-handed helix found in dehydrated conditions.
  * **Z-DNA:** The elongated, left-handed helix with a distinct zig-zag sugar-phosphate backbone.
* **Detailed Chemical Ball-and-Stick View:** Switch to a fully accurate atomic model. By utilizing Three.js `PDBLoader`, the application fetches `1D68.pdb` (High-Resolution NMR structure). Unlike standard X-Ray files, this NMR model includes **all protons (Hydrogens)**. The engine calculates precise covalent bond distances (0.4Å to 1.75Å) to draw stunning physical sticks connecting every atom.
* **Dynamic Educational UI:** An overlay interface displays real-time structural data, biological descriptions, and dynamic color legends as you switch modes.

## 🛠️ Technologies Used
* **HTML5 / CSS3:** For the layout and glass-morphic user interface.
* **Vanilla JavaScript (ES6+):** For application state logic and dynamic molecular algorithms.
* **Three.js:** Core 3D library processing the mathematical rotations, square-distance bond vector mathematics, and handling lighting/materials.
* **RCSB PDB API:** Direct connection to fetch true high-definition structural atomic coordinates.

## 🚀 How to Run Locally
Because this project is entirely front-end and relies on a CDN for scripts, there is no build step or package installation required!

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   ```
2. Navigate to the folder:
   ```bash
   cd <your-repo-name>
   ```
3. Open the `index.html` file in any modern web browser (Chrome, Firefox, Safari, Edge). *Note: An active internet connection is required to fetch the Three.js libraries and the chemical PDB file.*

## 🌐 Hosting on GitHub Pages
This repository is pre-configured to be hosted easily on GitHub Pages.
1. Upload your `index.html` file to your GitHub repository.
2. Go to your repository **Settings** > **Pages**.
3. Under "Build and deployment", select **Deploy from a branch**.
4. Set the branch to `main` (or `master`), select the `/ (root)` folder, and click **Save**.
5. Your interactive model will be live in a few minutes!

## 🔬 Scientific Legend

### Abstract Procedural View
* 🟥 **Adenine (A)**
* 🟦 **Thymine (T)**
* 🟩 **Cytosine (C)**
* 🟨 **Guanine (G)**
* ⬜ **Sugar-Phosphate Backbone**

### Detailed NMR Atomic View (CPK Colors)
* ⚪ **Hydrogen (H)**
* 🔘 **Carbon (C)**
* 🔴 **Oxygen (O)**
* 🔵 **Nitrogen (N)**
* 🟠 **Phosphorus (P)**
* ◽ **Covalent Bonds**

## 📝 License
This project is open-source and available under the MIT License. Feel free to use, modify, and distribute it for educational purposes.
