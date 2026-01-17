# University Department Website

**Project:** University Department Website — static website  
**Team Lead:** Khizra Jamshaid  
**Repo:** https://github.com/DevOpsProjectsG4/university-departments-site.git

---

## Overview
This project delivers a professional static website for the Computer Science Department of a university. The primary objective is not complex application logic, but hands-on mastery of modern DevOps practices—from containerization to automated multi-environment deployment. The website acts as an information portal for current students, faculty members and prospective applicants. All content is static, structured, and meaningful, built using HTML and CSS, containerized with Docker, and deployed automatically via CI/CD pipelines.

## Structure
```
university-departments-site/
├── .github/
│   └── workflows/
│       ├── ci-dev.yaml
│       ├── cd-dev.yaml
│       ├── ci-stage.yaml
│       ├── cd-stage.yaml
│       ├── ci-prod.yaml
│       └── cd-prod.yaml
├── assets/
│   └── logo.jpg
├── src/
│   ├── index.html
│   ├── courses.html
│   ├── faculty.html
│   ├── admissions.html
│   ├── contact.html
│   └── research.html
├── styles/
│   ├── index.css
│   ├── courses.css
│   ├── faculty.css
│   ├── admissions.css
│   ├── contact.css
│   ├── research.css
│   └── global.css
├── .gitignore
├── .dockerignore
├── .htmlhint.json
├── .stylelintrc.json
├── Dockerfile
├── package.json
└── README.md

```


## Setup Instructions

### Clone the repository 
```bash
git clone https://github.com/DevOpsProjectsG4/university-departments-site.git
cd university-departments-site
```

### Install Node.js dependencies
Make sure you have Node.js installed. Then run:
```bash
npm install
```
### Lint HTML files in your code
```bash
npx htmlhint "**/*.html"
```
### Lint CSS files on your code
```bash
npx stylelint "**/*.css"
```
### Build your code
```bash
npx parcel build "./src/index.html" --dist-dir "./dist" --public-url "./" --no-cache
```