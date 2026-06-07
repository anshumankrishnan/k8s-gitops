# PHASE 5 - SECURITY (TRIVY)

## Tool Used
Trivy by Aqua Security

## Image Scanned
anshuman0789/k8s-app:v2

## Scan Type
- Vulnerability scan
- Secret scan

## Summary
- OS: Alpine Linux
- Packages scanned successfully
- Node.js dependencies scanned

## Findings
- Low/medium vulnerabilities may exist (normal for base images)
- Image uses public Docker Hub registry (acceptable for assignment but not production-safe)

## Security Notes
- Always use minimal base images
- Regularly update dependencies
- Use private registry in production
- Add image scanning in CI pipeline

## Output File
trivy-report.txt
