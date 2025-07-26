# static-website

Lab 4: CI/CD with GitHub Actions for a Fullstack Project

Objective: Automate Build, Test, and Deploy Tasks using GitHub Actions for Fullstack Projects and make it live on GitHub Pages.
What is GitHub Actions?
•  GitHub Actions is a CI/CD automation tool built into GitHub.
•  It allows you to build, test, and deploy your code automatically whenever changes happen (e.g., on push, pull request).
•  It uses YAML-based workflows stored in .github/workflows/.
Why GitHub Actions for Fullstack Projects?
•  Seamless with GitHub (no extra installation)
•  Enables automated CI/CD pipelines for both frontend and backend code
•  Supports parallel jobs, caching, notifications, and deployment steps
 ***Workflow Structure (YAML)

 
 Folder Structure
fullstack-app/
├── backend/     → Node.js/Java Spring Boot code
│   └── package.json / pom.xml
├── frontend/    → React/Vue/Angular code
│   └── package.json
└── .github/
    └── workflows/
        └── ci-cd.yml

Step-by-Step: Creating GitHub Actions Workflow
  Step 1: Prepare your GitHub Repository
•  Code is organized with separate /frontend and /backend directories.
•  Each has its own package.json or pom.xml (if using Maven).

 Step 2: Add GitHub Actions Workflow File
1.  In your repo, create:
2.  .github/workflows/ci-cd.yml
3.  Paste the workflow YAML code .
Step 3: Commit and Push
git add .
git commit -m "Add GitHub Actions CI/CD workflow"
git push origin main

Step 4: Monitor Workflow in GitHub
1.  Go to your GitHub repository
2.  Click on Actions tab
3.  You will see the workflow running after the push
4.  View logs of each job (frontend and backend)

Step 5: Configure GitHub Pages
1.Go to your repo main page
2.Click "Settings" (top menu)
3. click "Pages" 
4.Under “Source”, select:
Branch: gh-pages
Folder: / (root)
Click "Save"
Step 6: Check Deployment
1.Go to Actions tab (top menu)
2.You’ll see your workflow running as a yellow dot or green tick
3.Once green, go back to Settings > Pages
4.Under “Your site is live at”, click the link!
