<p align="center">
  <img src="https://img.shields.io/badge/RepoSage-Contributing%20Guide-blueviolet?style=for-the-badge&logo=github" alt="Contributing Guide" />
  <br/>
  <strong>🚀 Your guide to contributing to the AI-powered developer copilot</strong>
</p>

<p align="center">
  <a href="https://github.com/kalyan-1845/ai-code-reviewer/issues"><img src="https://img.shields.io/github/issues/kalyan-1845/ai-code-reviewer?style=flat-square&color=orange" alt="Open Issues" /></a>
  <a href="https://github.com/kalyan-1845/ai-code-reviewer/pulls"><img src="https://img.shields.io/github/issues-pr/kalyan-1845/ai-code-reviewer?style=flat-square&color=blue" alt="Open PRs" /></a>
  <a href="CODE_OF_CONDUCT.md"><img src="https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa?style=flat-square" alt="Code of Conduct" /></a>
</p>

---

# Contributing to RepoSage 🚀

First off, **thank you** for considering contributing to **RepoSage**! It's contributors like you that make this AI-powered developer copilot so powerful.

We are officially participating in **GirlScript Summer of Code (GSSoC) 2026**! Whether you are a beginner or an experienced developer, we are thrilled to have you here. Every contribution matters — from fixing a typo to building a new feature.

> **💡 New to open source?** Don't worry! We have issues labeled `good-first-issue` specifically designed for newcomers. Our maintainers are friendly and happy to guide you through the process.

---

## 📋 Table of Contents

- [Getting Started](#-getting-started)
- [Development Setup](#-development-setup)
- [GSSoC '26 Contribution Workflow](#-gssoc-26-contribution-workflow)
- [Issue Labels](#-issue-labels)
- [Code Style Guidelines](#-code-style-guidelines)
- [PR Review Checklist](#-pr-review-checklist)
- [Recognition & Rewards](#-recognition--rewards)
- [Thank You](#-thank-you)

---

## 🛠 Getting Started

Before you begin, make sure your development environment meets the following prerequisites:

| Requirement | Minimum Version | Purpose |
|---|---|---|
| **Node.js** | `v18.0+` | Frontend & Backend runtime |
| **Python** | `3.10+` | AI Engine (FastAPI) |
| **npm** | `v9.0+` | Package management |
| **Git** | `v2.30+` | Version control |

You can verify your setup by running:

```bash
node -v      # Should print v18.x or higher
python --version  # Should print 3.10 or higher
npm -v       # Should print 9.x or higher
git --version    # Should print 2.30 or higher
```

---

## 🖥 Development Setup

RepoSage is a monorepo with **three modules**. Follow these steps to get each one running locally:

### 1️⃣ Fork & Clone the Repository

```bash
# Fork the repo on GitHub, then clone your fork
git clone https://github.com/<your-username>/ai-code-reviewer.git
cd ai-code-reviewer
```

### 2️⃣ Frontend (React)

```bash
cd frontend
npm install
npm run dev
```

The frontend dev server will start at `http://localhost:5173` (or as configured).

### 3️⃣ Backend (Node.js / Express)

```bash
cd backend
npm install
npm start
```

The backend API will start at `http://localhost:3000` (or as configured).

### 4️⃣ AI Engine (Python / FastAPI)

```bash
cd ai-engine
pip install -r requirements.txt
uvicorn app:app --reload
```

The AI engine will start at `http://localhost:8000`.

> [!TIP]
> Use a Python virtual environment (`python -m venv venv`) to avoid dependency conflicts.

---

## 🏷️ GSSoC '26 Contribution Workflow

To ensure a smooth collaboration process, please follow these steps:

1. **🔍 Find an Issue**
   Browse our open issues on GitHub or check [GOOD_FIRST_ISSUES.md](GOOD_FIRST_ISSUES.md). Look for the `gssoc26` and `good-first-issue` labels.

2. **🙋 Request Assignment**
   Comment on the issue stating your interest. Please wait for a Project Admin or Mentor to officially assign the issue to you before writing code. *We will not review or merge PRs from unassigned contributors to avoid duplicate work.*

3. **🍴 Fork & Clone**
   Fork the repository to your account and clone it locally.

4. **🌿 Create a Feature Branch**
   ```bash
   git checkout -b feat/issue-description
   # Example: git checkout -b feat/clipboard-copy
   ```

5. **💻 Develop & Test**
   Run the modules locally to verify your changes. Make sure your changes compile cleanly.
   - **Frontend:** `npm run dev` or `npm run build` to verify.
   - **Backend:** `npm start`
   - **AI Engine:** `uvicorn app:app --reload`

6. **📝 Commit & Push**
   Use semantic commit messages:
   ```bash
   feat(frontend): add copy code button to code viewer
   fix(backend): resolve GitHub auth token refresh issue
   docs: update API endpoint documentation
   ```

7. **🚀 Submit a Pull Request**
   Submit your PR targeting the `main` branch.
   - Reference the issue number in your PR description (e.g., `Closes #12`).
   - Provide screenshots or GIFs of UI changes where possible.
   - Fill out the PR template completely.

---

## 🏷️ Issue Labels

We categorize tasks using the following GitHub labels:

| Label | Description |
|---|---|
| `gssoc26` | Official GirlScript Summer of Code '26 tasks |
| `good-first-issue` | Simple tasks ideal for beginners |
| `documentation` | Enhancing READMEs, guides, or API specifications |
| `frontend` | React & CSS-related enhancements |
| `backend` | Express.js API & system logic |
| `ai-engine` | Python FastAPI & LLM prompts |

---

## 🛠️ Code Style Guidelines

- **Frontend (React):** Write reusable functional components, use clean CSS styling, and ensure responsive layouts.
- **Backend (Node.js):** Use asynchronous JavaScript (`async/await`) and handle errors gracefully.
- **AI Engine (Python):** Ensure compliance with PEP 8 and include descriptive type annotations.

---

## ✅ PR Review Checklist

Before submitting your Pull Request, please verify the following:

- [ ] 🔗 My PR is linked to an assigned issue (e.g., `Closes #XX`)
- [ ] 🌿 I created a feature branch from `main` (not committing directly)
- [ ] 🧪 I have tested my changes locally and they work as expected
- [ ] 🏗️ My code compiles/builds without errors or warnings
- [ ] 📱 UI changes are responsive and tested across screen sizes
- [ ] 🖼️ I have included screenshots/GIFs for any visual changes
- [ ] 📝 I used semantic commit messages (`feat:`, `fix:`, `docs:`, etc.)
- [ ] 📖 I have updated relevant documentation (if applicable)
- [ ] 🔒 I have not committed any API keys, secrets, or credentials
- [ ] 🤝 My code follows the project's [Code Style Guidelines](#-code-style-guidelines)
- [ ] 🧹 I have removed any console.log / debug statements

---

## 🏆 Recognition & Rewards

We believe in celebrating our contributors! Here's how we recognize your efforts:

| Contribution | GSSoC Points | Badge |
|---|---|---|
| Documentation / Typo Fix | ⭐ Level 1 (10 pts) | 📝 Docs Hero |
| Bug Fix / Small Enhancement | ⭐⭐ Level 2 (25 pts) | 🐛 Bug Squasher |
| Feature Implementation | ⭐⭐⭐ Level 3 (45 pts) | 🚀 Feature Builder |

> **🏅 GSSoC Leaderboard:** All accepted PRs contribute to your GSSoC '26 leaderboard score. The more impactful your contributions, the higher you climb!

**Additional Perks:**
- 🎖️ Featured on our [Contributors Wall](https://github.com/kalyan-1845/ai-code-reviewer#contributors) in the README
- 📜 Certificate of contribution from GSSoC '26
- 💼 Real-world experience with AI, React, Node.js, and Python
- 🌐 Networking with a growing open-source community

---

## 💬 Need Help?

- 💬 Open a [GitHub Discussion](https://github.com/kalyan-1845/ai-code-reviewer/discussions) for questions
- 🐛 Report bugs via [GitHub Issues](https://github.com/kalyan-1845/ai-code-reviewer/issues)
- 📧 Reach the maintainer at **bhoompallykalyanreddy@gmail.com**

---

## 🙏 Thank You

<p align="center">
  <img src="https://img.shields.io/badge/Thank%20You-Contributors!-ff69b4?style=for-the-badge&logo=heart" alt="Thank You" />
</p>

A heartfelt **thank you** to every contributor who has helped make RepoSage better! Your time, effort, and creativity are what drive this project forward. Whether you fixed a bug, improved documentation, or built a brand-new feature — **you are awesome**. 🌟

Every contribution, no matter how small, makes a real difference. Together, we're building something incredible for the developer community.

Please respect our [Code of Conduct](CODE_OF_CONDUCT.md) in all communication channels. Happy hacking! 💻🔥

<p align="center">
  Made with ❤️ by the <strong>RepoSage</strong> community
</p>
