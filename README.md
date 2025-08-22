# Elome Govt Websites 🌐

This is the **Elome Govt Websites** project, deployed using **Firebase Hosting** and automated with **GitHub Actions**.

---

## 🚀 Deployment Setup

This project is automatically deployed to **Firebase Hosting** whenever code is pushed to the `main` branch.

### 🔑 Firebase Authentication
We use a Firebase **Service Account Key** stored securely in **GitHub Secrets**.

1. Go to **Firebase Console** → `Project Settings` → `Service Accounts`.
2. Click **Generate new private key** and download the JSON file.
3. In GitHub → Repository → **Settings** → **Secrets and variables** → **Actions** → Add a new secret:
   - **Name:** `FIREBASE_SERVICE_ACCOUNT_ELOME_GOVT_WEBSITES`
   - **Value:** *(entire JSON content from the Firebase key file)*

---

## ⚡ GitHub Actions Workflow

- The workflow file is located at:  
  `.github/workflows/firebase-hosting-merge.yml`

- On every push to `main`, it:
  1. Installs dependencies
  2. Builds the project
  3. Deploys to Firebase Hosting

You can check the logs under the **Actions tab** in GitHub.

---

## 🌍 Live Website
Once deployed, the website will be available at:

👉 [https://elome-govt-websites.web.app/](https://elome-govt-websites.web.app/)  

(Or your custom domain if configured)

---

## 🛠️ Tech Stack
- **Frontend:** HTML, CSS, JavaScript (add framework if used, e.g., React, Vue, etc.)
- **Hosting:** Firebase Hosting
- **CI/CD:** GitHub Actions

---

## 📜 License
This project is licensed under the **MIT License** – feel free to use and modify.
