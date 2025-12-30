# ML-Playground

Hands‑on Jupyter notebooks for learning core ML concepts (overfitting, underfitting) and TensorFlow — runnable in Colab.

Topics
machine-learning, tensorflow, colab, jupyter-notebook, tutorials, overfitting, underfitting, beginner-ml

---

Table of Contents
- About
- Features
- Notebooks (highlights)
- Quick start (Colab)
- Run locally
- Project structure
- Examples
- Contributing
- License
- Contact

About
This repo contains concise, well-documented Jupyter notebooks that demonstrate fundamental machine learning concepts and practical TensorFlow workflows. It's aimed at learners who want runnable examples they can open in Colab, tweak, and experiment with — with emphasis on intuition (e.g., overfitting/underfitting), model building, training loops, evaluation, and visualizations.

Features
- Clear, short notebooks focused on a single concept
- Ready-to-run in Google Colab (no local setup required)
- Vanilla TensorFlow / Keras examples and common baselines
- Visualizations to illustrate training dynamics (loss, accuracy, overfitting)
- Tips, "what went wrong" sections, and suggested exercises
- Minimal dependencies (can run locally with a small requirements file)

Notebooks (highlights)
- notebooks/01-linear-regression.ipynb — Simple linear regression from scratch and with Keras
- notebooks/02-logistic-regression.ipynb — Binary classification, decision boundary visualization
- notebooks/03-overfitting-underfitting.ipynb — Demonstrates model capacity, regularization, and data size effects
- notebooks/04-cnn-mnist.ipynb — Convolutional neural network on MNIST with augmentation
- notebooks/05-transfer-learning.ipynb — Transfer learning with a pre-trained model (TensorFlow Hub)
- notebooks/99-exercises.ipynb — Suggested exercises and extension ideas

Quick start — Open in Colab (recommended)
Click any notebook's "Open in Colab" badge or use the link pattern below to open a notebook directly in Colab:

Open a notebook in Colab:
https://colab.research.google.com/github/SindhuraShankeshi/ML-Playground/blob/main/notebooks/01-linear-regression.ipynb

(Replace the file name at the end to open a different notebook.)

Run locally (if you prefer)
1. Clone the repo:
   git clone https://github.com/SindhuraShankeshi/ML-Playground.git
   cd ML-Playground

2. (Optional) create and activate a virtual environment:
   python -m venv .venv
   source .venv/bin/activate   # macOS / Linux
   .venv\Scripts\activate      # Windows (PowerShell)

3. Install dependencies:
   pip install -r requirements.txt

4. Start Jupyter:
   jupyter notebook   # or jupyter lab

Notes:
- requirements.txt contains minimal packages (tensorflow, matplotlib, numpy, pandas, scikit-learn).
- If you want GPU acceleration locally, install the appropriate TensorFlow build for your platform and CUDA version or use a GPU-enabled Colab runtime.

Project structure
- notebooks/        — Jupyter notebooks (primary content)
- data/             — small datasets or download scripts (if included)
- examples/         — helper scripts for quick demos (optional)
- assets/           — images, diagrams, screenshots used in notebooks/README
- requirements.txt  — Python dependencies
- LICENSE
- README.md

Examples and usage tips
- Overfitting vs underfitting: `03-overfitting-underfitting.ipynb` progressively increases model capacity and shows training vs validation curves, demonstrates dropout/L2 regularization, and explores dataset size effects.
- Quick experiments: edit hyperparameters (learning rate, batch size, model depth) and re-run cells to see immediate results.
- Visual debugging: each training example includes plots of loss/accuracy and sample predictions.

Contributing
Contributions, issues, and suggestions are welcome! Suggested workflow:
1. Fork the repo
2. Create a branch: git checkout -b feature/your-feature
3. Add or improve a notebook, include a short description and learning objective at the top
4. Add tests or a minimal example if applicable (notebooks should run end-to-end)
5. Commit and open a pull request with context and screenshots (if UI/plot changes)

Guidelines for new notebooks
- Keep notebooks focused on a single concept or short workflow
- Include an objectives section at the top
- Use small datasets or clearly document dataset download instructions
- Aim for reproducibility: set random seeds where helpful and note expected runtimes
- Prefer clear visualizations and brief commentary over long prose

Roadmap / ideas
- More examples on time series, NLP basics, and evaluation metrics
- Interactive widgets to tweak hyperparameters
- Dockerfile or Binder configuration for reproducible environments
- A short pedagogical blog-style explanation accompanying each notebook

License
MIT License — see LICENSE file.

Contact
Created by SindhuraShankeshi. For questions or suggestions, open an issue or PR.

Acknowledgements
- Built with TensorFlow and the browser/runtime of your choice (Colab recommended for quick experiments).
- Thanks to the open-source community for datasets and tooling.

If you'd like, I can:
- generate all notebook skeletons and a minimal requirements.txt,
- add Colab badges to each notebook with correct links,
- or create a Binder/Voila configuration for instant demos — tell me which and I'll create the files.
