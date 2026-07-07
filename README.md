# RHEL Server Hardening
 
A hands-on project where I set up a RHEL 10.2 server and took it through a full hardening and audit cycle — user access control, SSH key-based login, centralized logging, backups, patch management, and a manual security review.
 
Built as a practical companion to a Red Hat Admin 1 course and Samsung Innovation Campus material, applying each concept to one real server instead of isolated exercises.
 
## What's in here
 
- **`docs/`** — six phase-by-phase pdf documents with real command output and screenshots, covering setup, users, SSH, logging, backups, and the final security audit
- **`report/`** — a short summarized pdf report pulling the whole project together
## Highlights
 
- Role-based users and groups, with password aging policy and a two-layer offboarding lock
- SSH hardened to key-only login, verified against server auth logs
- A real diagnosed issue: a test log message went missing until I traced it to RHEL's default routing rules
- Persistent journald logging, backups via tar/xz, and patch management treated as a security task
- A manual audit that actually caught something — an SGID script sitting in a non-standard location
## Environment
 
RHEL 10.2, registered with Red Hat, single VM.
 
## Author
 
Lobna Ahmed
