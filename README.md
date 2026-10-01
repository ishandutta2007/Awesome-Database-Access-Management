# Awesome-Database-Access-Management

# Top Database Access Management Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Privileged Access Management, Just-in-Time Database Access & Audit Compliance*
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Database Access Management**. These tools help organizations control, monitor, and audit access to databases and other critical infrastructure—eliminating standing privileges, enabling just-in-time (JIT) access, and providing full session visibility for compliance.

**Examples** include StrongDM, Teleport, Axiomatics, HashiCorp Boundary, DataSunrise, One Identity Safeguard, ManageEngine PAM360, CyberArk, and Delinea (the category leaders).

**Open-source emphasis**: Database access management has a **mature and production-proven open-source ecosystem**. **Teleport** provides a comprehensive open-core PAM platform with database access, SSH, Kubernetes, and application access . **JumpServer** (27,930 stars) is the leading open-source PAM with web-based access to SSH, RDP, Kubernetes, and databases . **Thand** delivers distributed just-in-time access management with serverless workflows and Temporal orchestration . **CloudDM** provides an open-source database management console with RBAC and approval workflows . This section documents these production-grade solutions.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[StrongDM](https://www.strongdm.com/)**
  **Zero Trust Privileged Access Management (PAM) platform for modern infrastructure.** Combines authentication, authorization, networking, and observability into a single platform for databases, servers, Kubernetes, clouds, and web applications . **Key features**: No credentials on user machines (credentials fetched from vault on-demand); JIT access via Access Workflows; complete protocol support for SSH, RDP, Kubernetes, and databases; full session recording and replay; granular RBAC; SSO integration; Terraform provider and SDKs in Go, Java, Python, Ruby . **Deployment**: SaaS with local client, no software deployed to resources .

- **[Teleport](https://goteleport.com/)**
  **Open-core PAM platform with comprehensive database access.** Provides secure access to PostgreSQL, MySQL, MongoDB, Redis, Cassandra, ClickHouse, CockroachDB, DynamoDB, Microsoft SQL Server, Oracle, OpenSearch, and Snowflake . **Key features**: Short-lived certificates via SSO (eliminates shared secrets); RBAC with object-level permissions (table/schema level); automated user provisioning (each user gets own DB account); session recording and audit; Access Requests workflow . **Open-core** with enterprise features; also available as commercial SaaS.

- **[Axiomatics](https://www.axiomatics.com/)**
  Dynamic authorization and fine-grained access control platform. Provides attribute-based access control (ABAC) for databases and applications.

- **[HashiCorp Boundary](https://www.hashicorp.com/products/boundary)**
  Identity-based access management for dynamic infrastructure. Provides secure remote access to databases and systems without exposing credentials.

- **[DataSunrise](https://www.datasunrise.com/)**
  Database security and compliance platform. Provides database activity monitoring, dynamic data masking, and database firewall capabilities.

- **[One Identity Safeguard](https://www.oneidentity.com/)**
  Privileged access management platform with database access control, session recording, and credential vaulting.

- **[ManageEngine PAM360](https://www.manageengine.com/)**
  Complete privileged access management solution. Provides privileged account management, session monitoring, and database access control.

- **[CyberArk](https://www.cyberark.com/)**
  Industry-leading PAM platform. Provides privileged account security, session isolation, and database access management.

- **[Delinea](https://delinea.com/)**
  PAM platform (formerly Thycotic and Centrify). Provides privileged access management, credential vaulting, and database access control.

## Open-Source GitHub Projects

### Comprehensive PAM Platforms

- **[JumpServer](https://github.com/jumpserver/jumpserver)**
  **The leading open-source Privileged Access Management (PAM) platform.** **27,930 stars, 5,494 forks**, **GPL-3.0 licensed**, Python-based . Provides DevOps and IT teams with on-demand secure access to **SSH, RDP, Kubernetes, Database, and RemoteApp endpoints through a web browser** . **Key capabilities**: Web-based access console; session recording and replay; credential vaulting; RBAC; multi-tenancy; audit logging. **Deployment**: Self-hosted; active development (updated 4 days ago as of search) . **Best for**: Organizations needing a comprehensive open-source PAM with web-based access to multiple protocols.

- **[Teleport](https://github.com/gravitational/teleport)**
  **Open-core PAM platform with the most comprehensive database protocol support.** **Open-core model** — core is open-source, enterprise features available commercially. Provides database access with short-lived certificates, RBAC with object-level permissions, and full session recording . **Key differentiator**: Cryptographically secure certificates eliminate shared secrets; sessions automatically expire; automated user provisioning for per-user database accounts . **Best for**: Teams wanting self-hosted database access management with strong compliance features.

### Just-in-Time (JIT) Access

- **[Thand Agent](https://github.com/thand-io/agent)**
  **Distributed open-source agent for Privileged Access Management (PAM) and Just-in-Time (JIT) access.** **BSL 1.1 licensed** . **Core innovation**: Uses **Serverless Workflows and Temporal** to orchestrate and guarantee deterministic workflow execution and revocation of permissions across cloud/on-prem environments . **Key features**: **Zero standing privileges** (no permanent admin access); **No static credentials** (all access temporary, tied to identity); **JIT permissions** (request access when needed, automatically revoked after use); complete audit trail; automatic access review during usage . **Deployment**: Self-hosted via Docker, Kubernetes, AWS Lambda, or GCP Cloud Function; or Thand Cloud for enterprise features . **Best for**: Organizations eliminating standing privileges across cloud and SaaS infrastructure.

### Database Management & Access Control

- **[CloudDM](https://github.com/edurt/CloudDM)**
  **Open-source database management tool for teams.** **Apache-2.0 licensed** . Provides a **web console for SQL queries, database management, access control, SQL auditing, approval workflows, and database CI/CD** . **Key features**: Supports MySQL, Oracle, StarRocks, and Apache Cloudberry; **work orders** for production database changes with submit/approve/execute workflow; **CI/CD integration** via Git Push, WebHook, HttpCall; **RBAC** for team collaboration with role-based access to data sources and operations . **Best for**: Teams needing database access governance with approval workflows.

- **[DbGate](https://github.com/dbgate/dbgate)**
  **Cross-platform database manager (desktop and web).** **MIT licensed** (Community edition) . Supports MySQL, PostgreSQL, SQL Server, MongoDB, SQLite, Redis, MariaDB, CockroachDB, DuckDB, Firebird, and more . **Editions**: **Community** (free, open-source: connection, query, filtering, ER diagrams, export/import); **Premium** (query designer, charts, AI tools, master/detail views); **Team Premium** (self-hosted web with administration UI, users/roles/permissions, OAuth/OIDC) . **Note**: Some features moved from Community to Premium in v6.6.8 . **Best for**: Teams wanting a lightweight database management GUI with optional enterprise governance.

- **[Jaxon DbAdmin](https://github.com/lagdo/dbadmin-app-laravel)**
  **Web-based database management tool with multiple DBMS support and extensible authentication.** **BSD 3-Clause licensed** . **Features**: Browse servers/databases in tabs; query editor with retention; save queries and history; read credentials from secret managers; **audit logs** database with dedicated page and restricted access; import/export data; create/alter tables and views . **Best for**: Laravel/PHP applications needing embedded database administration.

### Additional Strong Open-Source Options

- **Comprehensive PAM**: **JumpServer** (27,930 stars, web-based access to SSH/RDP/K8s/DB) , **Teleport** (open-core, comprehensive database protocol support, object-level RBAC) .
- **JIT Access**: **Thand Agent** (distributed JIT, Temporal orchestration, zero standing privileges) .
- **Database Management**: **CloudDM** (RBAC, approval workflows, CI/CD) , **DbGate** (cross-platform, SQL + NoSQL) , **Jaxon DbAdmin** (web-based, audit logs) .
- **Alternatives**: **DBeaver** (16,828 stars, universal database tool), **Beekeeper Studio** (modern SQL client), **phpMyAdmin** (classic MySQL administration) .

**Frameworks for building custom systems**: Combine **Teleport** for database access with short-lived certificates and object-level RBAC, **JumpServer** for comprehensive PAM with web-based access to multiple protocols, **Thand Agent** for JIT access with zero standing privileges, and **CloudDM** for database management with approval workflows and CI/CD integration. Add **PostgreSQL** for audit persistence and **Docker/Kubernetes** for deployment.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Database access management platforms handle sensitive credentials and privileged access; ensure compliance with SOC 2, PCI DSS, HIPAA, and relevant regulatory requirements.
- **Open-source reality**: The open-source ecosystem for database access management is **mature and production-proven**. **JumpServer** provides comprehensive PAM with web-based access to multiple protocols and 27,930 stars . **Teleport** offers open-core database access with short-lived certificates, object-level RBAC, and comprehensive protocol support . **Thand Agent** delivers distributed JIT access with zero standing privileges . **CloudDM** provides database management with RBAC and approval workflows . However, **commercial platforms** (StrongDM, CyberArk, Delinea) provide **managed infrastructure, enterprise-grade integrations, dedicated support, and advanced features like AI agent governance** that open-source alternatives require significant operational investment to match . The open-source path is **genuinely viable** for organizations with strong security engineering capacity.

---

**Made for security engineers, database administrators, DevOps teams, and compliance officers.**
Let's make database access management more open, transparent, and secure.
