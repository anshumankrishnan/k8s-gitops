# 🚀 Production-Grade Kubernetes Platform

A complete cloud-native Kubernetes platform built using GitOps, CI/CD, Monitoring, Security Scanning, Disaster Recovery, and Infrastructure as Code practices.

---

## 📌 Project Overview

This project demonstrates the implementation of a production-style Kubernetes platform using modern DevOps and Cloud Engineering tools.

The platform includes:

- Kubernetes (K3s)
- GitOps with ArgoCD
- CI/CD with GitHub Actions
- Containerization with Docker
- Monitoring with Prometheus & Grafana
- Security Scanning with Trivy
- Disaster Recovery with ArgoCD Self-Healing
- Infrastructure as Code with Terraform
- Source Control with GitHub

---



# 🏗 Architecture

<img width="1172" height="654" alt="Screenshot 2026-06-08 130905" src="https://github.com/user-attachments/assets/1ea00cc6-2998-46d9-abb8-9a2d339f1cca" />

# ⚙️ Technology Stack

| Category | Tool |
|-----------|------|
| Containerization | Docker |
| Orchestration | K3s Kubernetes |
| GitOps | ArgoCD |
| CI/CD | GitHub Actions |
| Monitoring | Prometheus |
| Visualization | Grafana |
| Security | Trivy |
| IaC | Terraform |
| SCM | GitHub |
| Cloud Provider | AWS EC2 |

---

# 📂 Repository Structure

```text
k8s-gitops/
│
├── .github/
│   └── workflows/
│       └── ci-cd.yml
│
├── app/
│   ├── server.js
│   └── package.json
│
├── Dockerfile
├── deployment.yaml
├── service.yaml
│
├── SECURITY_REPORT.md
├── trivy-report.txt
│
└── README.md
```

---

# ☸ Kubernetes Deployment

Resources created:

- Deployment
- Service
- Replica Management
- Self-Healing Pods

Verify:

```bash
kubectl get pods
kubectl get svc
kubectl get deployments
```

---

# 🔄 GitOps with ArgoCD

Features implemented:

✅ Automated Sync

✅ Continuous Deployment

✅ Git as Single Source of Truth

✅ Self-Healing

✅ Drift Detection

Application Status:

```bash
kubectl get application k8s-app -n argocd
```

Expected:

```text
SYNC STATUS: Synced
HEALTH STATUS: Healthy
```

---

# 📊 Monitoring Stack

Monitoring tools deployed:

### Prometheus

Collects:

- Node Metrics
- Pod Metrics
- Kubernetes Metrics

### Grafana

Dashboards:

- CPU Usage
- Memory Usage
- Node Health
- Pod Status

Verify:

```bash
kubectl get pods -n monitoring
```

---

# 🔐 Security Scanning

Security implemented using Trivy.

Scanned:

- Docker Images
- Kubernetes Manifests

Reports:

```text
SECURITY_REPORT.md
trivy-report.txt
```

Run scan:

```bash
trivy image anshuman0789/k8s-app:v2
```

---

# 🚀 CI/CD Pipeline

GitHub Actions Pipeline performs:

1. Checkout Source Code
2. Build Docker Image
3. Security Scan with Trivy
4. Push Image to Docker Hub
5. Update Kubernetes Manifest
6. Trigger ArgoCD Deployment

Workflow Location:

```text
.github/workflows/
```

---

# 🔄 Disaster Recovery

Disaster recovery tested using ArgoCD Self-Healing.

Simulation:

```bash
kubectl delete deployment k8s-app
```

Result:

```text
ArgoCD automatically recreated the deployment.
```

This validates:

- Self-Healing
- Automatic Recovery
- GitOps Reconciliation

---

# 🌍 Infrastructure as Code

Terraform used for:

- AWS EC2 Provisioning
- Security Group Creation
- Automated Infrastructure Deployment

Commands:

```bash
terraform init
terraform plan
terraform apply
```

---

# 📸 Screenshots

- AWS EC2 Instance
<img width="1906" height="925" alt="Screenshot 2026-06-07 154307" src="https://github.com/user-attachments/assets/dbdbcb8a-6818-4539-956e-6dad12a57646" />

- K3s Node


- ArgoCD Dashboard
 <img width="1918" height="1091" alt="Screenshot 2026-06-06 142400" src="https://github.com/user-attachments/assets/d69db2c3-84ef-437e-a593-ae016bea0e8c" />


- Prometheus Targets

<img width="1909" height="1091" alt="Screenshot 2026-06-06 162324" src="https://github.com/user-attachments/assets/d89881e4-8f59-4726-8fd9-3f560cbdf45c" />

- GitHub Actions Success

- <img width="1912" height="1026" alt="Screenshot 2026-06-07 143304" src="https://github.com/user-attachments/assets/6b4aded7-0c5c-4135-8a5b-bb8d06251c2e" />

- Trivy Scan Report
<img width="1117" height="1003" alt="Screenshot 2026-06-07 144226" src="https://github.com/user-attachments/assets/d07483fa-fcab-426d-925a-d9ab5800261c" />
 <img width="920" height="1074" alt="Screenshot 2026-06-07 144315" src="https://github.com/user-attachments/assets/231c1612-0a47-49df-8048-53b16205f505" />


---

# 🎯 Project Outcomes

Successfully implemented:

- Kubernetes Platform Engineering
- GitOps Workflow
- CI/CD Automation
- Monitoring & Observability
- Security Scanning
- Disaster Recovery
- Infrastructure as Code

---

# 📚 Key Learnings

- Kubernetes Administration
- GitOps Principles
- ArgoCD Operations
- Cloud Infrastructure Management
- Terraform Fundamentals
- DevSecOps Practices
- Monitoring & Observability
- Disaster Recovery Strategies

---

# 👨‍💻 Author

**Anshuman Krishnan**

Cloud Computing Student | DevOps Enthusiast | Platform Engineering Learner

GitHub:
https://github.com/anshumankrishnan

---

# ⭐ Project Status

✅ Infrastructure Provisioned

✅ Kubernetes Cluster Running

✅ Application Containerized

✅ GitOps Configured (ArgoCD)

✅ Monitoring Implemented (Prometheus + Grafana)

✅ Security Scanning Completed (Trivy)

✅ CI/CD Pipeline Operational (GitHub Actions)

✅ Disaster Recovery Tested (ArgoCD Self-Healing)

✅ Infrastructure as Code Implemented (Terraform)

✅ Production-Grade Kubernetes Platform Completed
