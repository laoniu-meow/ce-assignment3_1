# Assignment 3.1 - Introduction to DevSecOps & Workflows

- Set up a basic CI/CD pipeline using GitHub Actions to automate code builds and deployments.
- Integrate a security scanning tool (such as OWASP ZAP, SonarQube, or Trivy) into your pipeline to analyze security vulnerabilities.
- Take screenshots of your pipeline setup and results.

## How am I approaching the challenge of completing this assignment?

### Step 1: Repository Setup

- Create a repository on GitHub
- Clone to local repository

### Step 2: Next.js Application

- Execute: `npx create-next-app@latest ce-assignment3_1`
- Creates a modern React application with built-in tooling

### Step 3: Security Plugin (Optional)

- Execute: `npm install --save-dev eslint-plugin-security`
- Adds security rules to ESLint

### Step 4: GitHub Actions Setup

- Create workflow directory: `mkdir -p .github/workflows`
- Create workflow file: `touch .github/workflows/ci-cd.yaml`

### Step 5: CI/CD Configuration

- Define workflow in `ci-cd.yaml`
- Configure triggers, jobs, and steps

### Step 6: Local Testing

Before pushing code, test locally:

- ✅ npm run lint # Runs ESLint with Next.js rules
- ✅ npm run build # Builds your Next.js app
- ✅ npm run dev # Starts development server
- ✅ npm run start # Starts production server

### Step 7: Commit and push the code

## Screenshots

![Alt text](/public/image1.png)
![Alt text](/public/image2.png)

- ❌ Scan Failed
![Alt text](/public/image3.png)

- ✅ My Repo no image file, so tells Trivy to scan files
![Alt text](/public/)