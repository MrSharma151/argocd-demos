# ArgoCD Demos & Practice Repository

This repository contains **hands-on ArgoCD practice and demos** built while learning GitOps concepts and real-world ArgoCD usage. The goal of this repo is to demonstrate **practical ArgoCD features**, not application development.

All examples follow **GitOps principles**, where Git is the single source of truth and ArgoCD continuously reconciles the desired state.

---

## 🚀 What This Repository Covers

* UI-based, CLI-based, and Declarative application deployments
* App-of-Apps pattern (parent–child applications)
* ApplicationSets for template-based multi-app deployments
* ArgoCD Projects for governance and access control
* Email notifications using ArgoCD Notifications
* Image update workflows (Git-based)
* Monitoring-ready application manifests
* Multi-cluster GitOps (demo structure)

---

## 📁 Repository Structure

```text
app_of_apps/                # App-of-Apps (parent-child) pattern
applicationsets/            # ApplicationSet examples
applicationset-multi-app.yaml
cli_approach/               # CLI-based ArgoCD application deployments
declarative_approach/       # Pure declarative GitOps applications
ui_approach/                # UI-based ArgoCD application deployments
email_notifications/        # ArgoCD email notification setup
image_updater/              # Image update demo (GitOps style)
monitoring/                 # Monitoring-ready application manifests
multicluster-app.yml        # Multi-cluster deployment example
project-devops.yaml         # ArgoCD Project (AppProject) definition
parent-app.yaml             # Parent application for App-of-Apps
```

---

## 🧩 Key Concepts Demonstrated

### 1. Application Deployment Methods

* **UI Approach** – Deploy applications directly using ArgoCD UI
* **CLI Approach** – Deploy applications using `argocd` and `kubectl`
* **Declarative Approach** – YAML-based GitOps deployments

### 2. App-of-Apps Pattern

* Central parent application
* Multiple child applications managed via Git
* Scalable and production-friendly structure

### 3. ApplicationSets

* Git directory generator
* Template-based application creation
* Used to deploy multiple applications from a single manifest

### 4. ArgoCD Projects

* Repository restrictions
* Namespace and destination controls
* Used for governance and isolation

### 5. Notifications

* Email notifications for:

  * Successful deployments
  * Health degradation
  * Sync failures
* SMTP-based notification setup

### 6. Image Update & Monitoring Demos

* Git-based image updates
* Manifests compatible with monitoring stacks

---

## 🔐 Secrets Management

* Kubernetes Secrets are **not committed to Git**
* Secret manifests are excluded using `.gitignore`
* Secrets are applied manually or via external secret management

---

## 🎯 Purpose of This Repository

This repository is meant for:

* Learning ArgoCD in a **production-aligned way**
* Demonstrating GitOps workflows
* Interview preparation and portfolio showcase

It is **not intended for application source code**, only infrastructure and deployment manifests.

---

## 🛠️ Tools & Technologies Used

* ArgoCD
* Kubernetes (kind / AKS compatible)
* Git & GitHub
* Helm & Kustomize (integration demos)
* Docker

---

## 📌 Note

This repository evolves as new ArgoCD features are practiced. Each directory represents a **focused ArgoCD concept** implemented using best practices.

---

✅ **Status:** Active learning & hands-on practice repository
