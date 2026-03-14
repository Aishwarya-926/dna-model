# 🧬 Interactive 3D DNA Structural Simulator

[![GitHub Pages](https://img.shields.io/badge/Hosted_on-GitHub_Pages-blue?logo=github)](https://<your-username>.github.io/<your-repo-name>/)
[![Made with Three.js](https://img.shields.io/badge/Made_with-Three.js-black?logo=three.js)](https://threejs.org/)

**[👉 View the Live 3D Simulation Here](https://aishwarya-926.github.io/dna-model/)**



## 📖 Overview
This project is an interactive, browser-based 3D educational tool designed to answer the prompt: *"Prepare a model for the A, B, or Z forms of deoxyribonucleic acid."* 

Instead of a physical model, this project leverages the power of WebGL and **Three.js** to dynamically generate highly accurate 3D structural models of the three primary conformations of DNA: **A-DNA**, **B-DNA**, and **Z-DNA**.

## ✨ Features
* **Real-Time 3D Rendering:** Fully interactive molecule. You can rotate, pan, and zoom to inspect the molecular structure from any angle.
* **Three DNA Conformations:** 
  * **B-DNA:** The standard, right-handed Watson-Crick double helix.
  * **A-DNA:** The compressed, wider, right-handed helix found in dehydrated conditions, featuring highly tilted base pairs.
  * **Z-DNA:** The elongated, left-handed helix with a distinct zig-zag sugar-phosphate backbone.
* **Scientific Accuracy:** The models are generated using relative crystallographic parameters, accurately reflecting differences in:
  * Handedness (Left vs. Right)
  * Base pairs per turn
  * Helical diameter
  * Rise per base pair (vertical stretch)
  * Base tilt relative to the helical axis
* **Dynamic Educational UI:** An overlay interface displays real-time structural data and biological descriptions as you switch between the DNA forms.

## 🛠️ Technologies Used
* **HTML5 / CSS3:** For the layout and glass-morphic user interface.
* **Vanilla JavaScript (ES6+):** For the application logic and molecular generation algorithms.
* **Three.js:** A cross-browser JavaScript library and application programming interface used to create and display animated 3D computer graphics in a web browser using WebGL.

## 🚀 How to Run Locally
Because this project is entirely front-end and relies on a CDN for Three.js, there is no build step or package installation required!

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   ```
2. Navigate to the folder:
   ```bash
   cd <your-repo-name>
   ```
3. Simply open the `index.html` file in any modern web browser (Chrome, Firefox, Safari, Edge).

## 🌐 Hosting on GitHub Pages
This repository is pre-configured to be hosted easily on GitHub Pages.
1. Upload your `index.html` file to your GitHub repository.
2. Go to your repository **Settings** > **Pages**.
3. Under "Build and deployment", select **Deploy from a branch**.
4. Set the branch to `main` (or `master`), select the `/ (root)` folder, and click **Save**.
5. Your interactive model will be live in a few minutes!

## 🔬 Scientific Legend
The simulation uses the following color coding for the nitrogenous bases:
* 🟥 **Adenine (A)**
* 🟦 **Thymine (T)**
* 🟩 **Cytosine (C)**
* 🟨 **Guanine (G)**
* ⬜ **Sugar-Phosphate Backbone**

## 📝 License
This project is open-source and available under the MIT License. Feel free to use, modify, and distribute it for educational purposes.
