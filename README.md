# Campus Bites – Campus Cafeteria Information Website

A small, static website for the fictional university cafeteria **Campus Bites**.
Built collaboratively with Git and GitHub for **DevOps Fundamentals (SEST4663) – Assignment 01**.
Plain HTML and CSS only – no backend, no JavaScript framework.

## Project Structure

```
campus-cafeteria/
├── .gitignore
├── README.md
├── src/
│   ├── index.html      (Home)            – Team Lead
│   ├── menu.html       (Menu)            – Member 1
│   ├── deals.html      (Deals)           – Member 2
│   ├── order.html      (How to Order)    – Member 3
│   └── feedback.html   (Feedback)        – Member 4
└── styles/
    └── style.css       (shared stylesheet)
```

## Branching Strategy

| Branch | Purpose |
|---|---|
| `main` | Production-ready code. No direct pushes. PRs need **3 approvals**. |
| `develop` | Integration branch for all active development. No direct pushes. PRs need **2 approvals**. |
| `feature/<page-name>` | One per member, created from `develop`. |
| `release/v1.0` | QA / testing branch cut from `develop`, merged into `main` then back into `develop`. |

## Workflow

1. Clone the repo and create `feature/<page-name>` from `develop`.
2. Commit small, descriptive changes; push the branch.
3. Open a Pull Request into `develop` (reviewers: teammates, assignee: Team Lead).
4. Before merging: `git fetch origin && git rebase origin/develop`, resolve conflicts, `git push --force-with-lease`.
5. Merge after 2 approvals.
6. Team Lead cuts `release/v1.0`, team tests, PR into `main` (3 approvals), then merges back into `develop`.

## Running Locally

Open `src/index.html` in any browser. All pages link to `../styles/style.css`.

## Team

See Table 1 in the assignment submission document.
