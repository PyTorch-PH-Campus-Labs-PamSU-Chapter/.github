# Forefront Page of PyTorch Philippines Campus Labs — Pampanga State University Chapter

This repository serves as the central administrative and community health repository for the **PyTorch Philippines Campus Labs - PSU Chapter** GitHub organization. It powers the organization landing page, global community templates, and chapter-wide contributor workflows.

---

## 📂 Repository Architecture

Because this repository is named `.github`, GitHub automatically inherits its templates, guidelines, and health files across **all repositories** in the organization that do not define their own local alternatives.

```text
.github/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.yml          # Form for runtime errors & script crashes
│   │   ├── feature_request.yml     # Form for new model architectures & topics
│   │   ├── task.yml                # Form for chapter deliverables & tasks
│   │   └── config.yml              # Form settings (disables blank issues)
│   └── PULL_REQUEST_TEMPLATE.md    # Global PR checklist inherited across all repos
├── profile/
│   └── README.md                   # Public landing page displayed on the org profile
├── CODE_OF_CONDUCT.md              # Organization-wide Code of Conduct & anti-hazing policy
├── CONTRIBUTING.md                 # Global developer & Git contribution workflow
└── README.md                       # Root documentation & handover guide (this file)
```

---

## ⚙️ How These Files Work Across the Organization

### 1. Organization Landing Page (`profile/README.md`)
* Any Markdown inside `profile/README.md` is rendered automatically on the public front page of the GitHub organization (`github.com/PyTorch-PH-Campus-Labs-PamSU-Chapter`).
* Update this file to feature active workshop series, link our social platforms, or display updated officer rosters.

### 2. Global Issue Forms (`.github/ISSUE_TEMPLATE/`)
* Any repository inside this GitHub organization will automatically display these YAML-based forms under the **Issues** tab.
* They provide visual web forms with text areas, dropdown menus, and validation rules so non-technical members and officers can submit actionable reports without writing Markdown or touching code.

### 3. Global Pull Request Template (`.github/PULL_REQUEST_TEMPLATE.md`)
* Automatically populates the description box whenever a contributor opens a Pull Request on any chapter repository.
* Enforces testing checklists, clean Python environment verification, and linked issues.

### 4. Community Health & Governance (`CODE_OF_CONDUCT.md` & `CONTRIBUTING.md`)
* **`CODE_OF_CONDUCT.md`:** Sets ethical standards, anti-hazing policies, and disciplinary escalation paths aligned with **Article X** of the Chapter Constitution.
* **`CONTRIBUTING.md`:** Standardizes Git branch conventions (`feat/`, `fix/`, `docs/`, `curriculum/`), PyTorch coding rules (device-agnostic setups, random seeds), and repository clean practices.

---

## 🔄 Officer Turnover & Maintenance Guide

For incoming **Technical Leads**, **Curriculum Coordinators**, and **Executive Board Members**:

1. **Permission Integrity:** 
   * Keep this repository restricted: only organization **Owners** and the **`Technical Core`** team should have maintain/write access.
   * Other Executive Board members retain `triage` access.
2. **Updating Forms:** 
   * When adding new dropdown items or questions to `.github/ISSUE_TEMPLATE/`, always validate the YAML formatting to ensure GitHub renders the web form properly.
3. **Overriding for Specific Repositories:** 
   * If a dedicated project needs custom forms or unique PR rules, simply create a local `.github/` folder inside that project's repository. GitHub will prioritize the local files over these global templates.

---

## 📜 Governance & Alignment
This repository is configured and maintained by the **Technical Lead** under the oversight of the **Technical and Communications Committee** and the **Executive Board**, in accordance with the official Constitution and By-Laws of the PyTorch Philippines Campus Labs - Pampanga State University Chapter.