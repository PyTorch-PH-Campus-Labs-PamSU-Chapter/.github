# 🤝 Contributing to PyTorch Campus Labs PSU

Thank you for your interest in contributing to the **PyTorch Philippines Campus Labs - Pampanga State University Chapter** codebases and learning materials! We welcome contributions from developers, researchers, and students of all experience levels.

---

## 🧭 Code of Conduct
By participating in this organization, you agree to abide by our [Code of Conduct](./CODE_OF_CONDUCT.md) and uphold the principles of inclusivity, integrity, and open-source collaboration.

---

## 🚀 Getting Started

### 1. Find or Open an Issue
* Before writing code, look through the repository's open **Issues**.
* If you have an idea or found a bug, submit an issue using our interactive forms:
  * 🐛 **Bug Report** — For broken code, library incompatibilities, or runtime errors.
  * 💡 **Feature Request** — For new models, starter kits, or tutorial topics.
  * 📋 **Task** — For chapter logistics or curriculum milestones.
* Wait for an assignment or thumbs-up from the **Technical Core** (`@PyTorch-PH-Campus-Labs-PamSU-Chapter/technical-core `) before starting substantial work.

### 2. Forking and Branching
1. Fork the target repository to your personal GitHub account.
2. Clone your fork locally:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```
3. Create a branch using our standard naming conventions:
   * `feat/<feature-name>` — New tutorials, models, scripts, or architectures.
   * `fix/<bug-name>` — Bug fixes and code corrections.
   * `curriculum/<topic-name>` — Notebooks, datasets, and workshop slides.
   * `docs/<topic-name>` — Documentation and README updates.

---

## 🛠️ Development & Coding Standards

### Python & PyTorch Best Practices
* **Reproducibility:** When training models, always set random seeds where possible (e.g., `torch.manual_seed(42)`).
* **Device Agnostic Code:** Write PyTorch scripts that run cleanly on CUDA, Apple Silicon (MPS), or CPU:
  ```python
  device = torch.device("cuda" if torch.cuda.is_available() else "mps" if torch.backends.mps.is_available() else "cpu")
  ```
* **Clean Environments:** Use virtual environments (`venv`, `conda`, or `uv`). Always update the `requirements.txt` or `pyproject.toml` when introducing new dependencies.
* **No Large Files:** **DO NOT** commit large datasets, model weight checkpoints (`.pth`, `.pt`, `.onnx` > 50MB), or sensitive API keys to the repository. Use Git LFS or provide download scripts in the documentation.

### Jupyter & Colab Notebooks
* Clear all output cells before committing notebooks (unless the repository explicitly requests pre-rendered outputs for tutorial reading).
* Ensure notebooks execute sequentially from top to bottom without relying on hidden execution states.

---

## 📥 Submitting a Pull Request (PR)

1. **Commit Messages:** Write concise, descriptive commit messages:
   * Good: `feat(vision): add resnet transfer learning tutorial`
   * Bad: `updates` or `fixed stuff`
2. **Push Your Branch:**
   ```bash
   git push origin feat/<feature-name>
   ```
3. **Open a PR:**
   * Target the `main` branch of the upstream chapter repository.
   * Fill out the automated **Pull Request Template**.
   * Link the issue being addressed (e.g., `Closes #14`).
4. **Code Review:**
   * The **Technical Core** will review your code.
   * Address any requested revisions promptly. Once approved and status checks pass, a maintainer will merge your PR.

---

## 💡 Need Help?
Have questions about setting up your environment or understanding a PyTorch script? Open a Discussion in the repo or reach out to the **Technical Lead** and **Curriculum Coordinator**.