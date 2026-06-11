# Security Engineering Roadmap — Checklist

Analyst → Security Engineer (DevSecOps) · 5–8 hrs/week · Jun 2026 → Jun 2027

## Week 1–2: GitHub & blog setup

- [x] Create `hmstk/hmstk` repo with profile README (template ready)
- [x] Update GitHub bio: "Security Engineer in progress — AWS · DevSecOps · Detection"
- [x] Delete or hide the `zero-to-mastery-captions-python` fork
- [ ] Set up SSH keys or fine-grained PAT for git
- [ ] Create `security-portfolio` repo with roadmap as README
- [x] Add About page to hamsteri.co (role, certs, GitHub link)

## Q1 (Jun–Aug 2026): Python + first project

- [ ] **Project 1 — AWS Security Auditor** (Python/boto3 CLI)
  - [ ] Scan: public S3 buckets
  - [ ] Scan: permissive security groups
  - [ ] Scan: IAM users without MFA
  - [ ] Scan: unencrypted EBS/RDS
  - [ ] JSON + HTML report output
  - [ ] README: problem → architecture → demo → how to run
- [ ] Add CI to Project 1: lint + unit tests + Gitleaks on every push
- [ ] Enable Dependabot + CodeQL on the repo
- [ ] Blog post #1: "Building an AWS security auditor in Python"
- [ ] Pin Project 1 on GitHub profile

## Q2 (Sep–Nov 2026): DevSecOps pipeline (flagship)

- [ ] **Project 2 — DevSecOps Reference Pipeline**
  - [ ] Pick target app (Juice Shop or small Flask app) and containerize it
  - [ ] Terraform to deploy to free-tier AWS
  - [ ] Pipeline stage: Gitleaks (secrets)
  - [ ] Pipeline stage: Semgrep (SAST)
  - [ ] Pipeline stage: Grype or Snyk (SCA)
  - [ ] Pipeline stage: Trivy (container scan)
  - [ ] Pipeline stage: Checkov (IaC scan)
  - [ ] Pipeline stage: OWASP ZAP baseline (DAST, post-deploy)
  - [ ] Fail build on criticals; publish SARIF to GitHub Security tab
  - [ ] Architecture diagram + threat model in README
- [ ] Blog post #2: pipeline walkthrough with real findings
- [ ] Pin Project 2

## Q3 (Dec 2026–Feb 2027): Kubernetes + detection

- [ ] **Dec checkpoint:** review progress — if behind, drop Project 4, protect Project 3
- [ ] **Project 3 — Kubernetes security lab** (kind/k3s)
  - [ ] Deploy Q2 app to local cluster
  - [ ] Network policies + Pod Security Standards
  - [ ] Trivy Operator
  - [ ] Falco runtime detection
  - [ ] Document 2–3 attack → detection scenarios
- [ ] Write 3–5 Sigma/Falco detection rules (malware-analysis bridge)
- [ ] Blog post #3: "Detecting container attacks with Falco"
- [ ] Pin Project 3

## Q4 (Mar–Jun 2027): Polish + job search

- [ ] **Project 4 — Reusable security tooling** (pick one)
  - [ ] Publish a GitHub Action to the Marketplace, OR
  - [ ] GuardDuty → Slack alerting Lambda
- [ ] Consistent READMEs across all repos (+ demo GIFs)
- [ ] Pin final 4 repos; link all from hamsteri.co
- [ ] Rewrite resume around the 4 projects
- [ ] LinkedIn headline → "Security Engineer"
- [ ] Start applying (month 10 — don't wait for "finished")
- [ ] Blog post #4: 12-month retrospective

## Ongoing (every week)

- [ ] 3+ small commits/week (contribution graph matters)
- [ ] Use Issues on your own repos to plan work

## Anti-goals (don't check these 🙂)

- No new certs for the first 6 months
- No parallel projects — one at a time
- No gold-plating — published 80% beats unpublished 100%
