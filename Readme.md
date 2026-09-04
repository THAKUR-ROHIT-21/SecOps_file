# DevSecOps

## What is DevSecOps?

**DevSecOps** means integrating security controls throughout the **Software Development Lifecycle (SDLC)** instead of treating security as a final manual stage.

The goal is to:

- Detect issues early
- Automate security checks in CI/CD
- Enforce security policies
- Continuously monitor production

---

# What DevSecOps Does in Daily at Work

## 1. Integrates Security into Development

DevSecOps integrates security practices directly into the software development process instead of checking security only at the end.

## 2. Perform SAST (Static Application Security Testing)

SAST is used to analyze source code or application code to identify security vulnerabilities before the application is deployed.

## 3. Perform SCA (Software Composition Analysis)

SCA is used to scan third-party dependencies, open-source libraries, and packages for known vulnerabilities.

## 4. Scan Secrets Leakage

Detects accidentally exposed secrets such as:

- API keys
- Passwords
- Tokens
- Access keys
- Credentials

## 5. Secure IaC

Infrastructure as Code is scanned to identify security misconfigurations in infrastructure definitions.

Examples:

- Terraform
- Kubernetes YAML
- CloudFormation
- Ansible

## 6. Scan Container

Container images are scanned for:

- OS vulnerabilities
- Package vulnerabilities
- Misconfigurations
- Security issues

## 7. Perform DAST (Dynamic Application Security Testing)

DAST tests a running application to identify security vulnerabilities from an external perspective.

## 8. Automate Security Checks in CI/CD

Security checks are integrated into CI/CD pipelines so that security testing happens automatically during the development and deployment process.

## 9. Enforce Security Gates

Security gates prevent insecure code, images, or deployments from progressing through the pipeline when they do not meet defined security requirements.

## 10. Monitors Application and Infrastructure

Continuously monitors applications and infrastructure for security-related events, suspicious activity, and operational issues.

## 11. Manage Vulnerabilities

Identifies, tracks, prioritizes, and helps remediate vulnerabilities across:

- Source code
- Dependencies
- Containers
- Infrastructure
- Applications

## 12. Code Quality Check

Performs automated code quality checks to identify:

- Bugs
- Code smells
- Maintainability issues
- Security issues

## 13. Code Smell Check

Identifies code smells and poor coding practices that can make applications difficult to maintain or potentially introduce problems.

## 14. CI/CD Scanning

Security scanning is integrated into CI/CD pipelines to continuously check:

- Source code
- Dependencies
- Secrets
- IaC
- Containers
- Applications
- Deployment configurations

---

# Tools and Tech Used by DevSecOps

## 1. Secure Code

**Tools:**

- SonarQube
- Checkmarx

Used for:

- Static code analysis
- Security vulnerability detection
- Code quality analysis

## 2. Scan Dependencies and Libraries

**Tools:**

- OWASP
- Snyk

Used to identify vulnerabilities in third-party dependencies and libraries.

## 3. Detect Secret

**Tools:**

- Gitleaks
- GitGuardian

Used to detect leaked secrets and credentials in source code and repositories.

## 4. Scan IaC

**Tools:**

- Trivy
- Checkov

Used to identify security misconfigurations in Infrastructure as Code.

## 5. Test Running Application

**Tools:**

- OWASP ZAP
- Burp Suite

Used for Dynamic Application Security Testing and identifying vulnerabilities in running applications.

## 6. Automate Security Checks

**Tools:**

- GitHub Actions
- GitLab CI/CD
- Jenkins

Used to automate security checks and integrate security into CI/CD pipelines.

## 7. Scan Container Image

**Tools:**

- Trivy
- Grype

Used to scan container images for vulnerabilities and security issues.

## 8. Block Insecure Deployment

**Tools:**

- SonarQube Quality Gates
- OPA (Open Policy Agent)

Used to enforce security and policy requirements and prevent insecure deployments.

## 9. Monitoring Production Security

**Tool:**

- Falco

Used to monitor runtime activity and detect suspicious behavior in production environments.

## 10. Manage Vulnerabilities

**Tools:**

- Snyk
- DefectDojo

Used to manage, track, prioritize, and monitor vulnerabilities.

---

# Main Tools

The main DevSecOps tools include:

- **SonarQube**
- **Trivy**
- **OWASP**
- **Gitleaks**
- **Falco**

---

# Core Concepts

## 1. Shift Left Security

**Shift Left Security** means moving security testing and security practices earlier into the Software Development Lifecycle.

Instead of finding vulnerabilities after deployment, security issues are identified during:

- Development
- Code commit
- Pull request
- Build
- CI/CD pipeline

---

## 2. Shift Right Security

**Shift Right Security** focuses on security after deployment and in production environments.

It includes:

- Runtime security
- Continuous monitoring
- Threat detection
- Incident response
- Production security testing

---

## 3. Defense in Depth

**Defense in Depth** means using multiple layers of security controls instead of depending on a single security mechanism.

Example:

```text
Developer
   ↓
Secure Code
   ↓
SAST
   ↓
SCA
   ↓
Secret Scanning
   ↓
IaC Scanning
   ↓
Container Scanning
   ↓
DAST
   ↓
Security Gate
   ↓
Deployment
   ↓
Runtime Monitoring