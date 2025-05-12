# DevOps Cheatsheet

## Was ist DevOps?

**Definition:** Eine Kultur und Praxis, die die Lücke zwischen Softwareentwicklung (Dev) und IT-Betrieb (Ops) schließt. Fokus auf **Kollaboration**, **Automatisierung** und **kontinuierliche Verbesserung**.

**Was DevOps NICHT ist:**
*   Kein spezifisches Tool oder Technologie.
*   Nicht nur Automatisierung (umfasst auch Kultur & Prozesse).
*   Kein separates Team (Integration von Dev & Ops).
*   Keine Einheitslösung (Anpassung nötig).
*   Kein Quick-Fix (eine Reise).
*   Nicht nur für große Unternehmen.

**Vorteile von DevOps:**
*   Schnellere Softwarelieferung & Deployment (CI/CD).
*   Verbesserte Zuverlässigkeit & Qualität (Autom. Testing, Monitoring).
*   Bessere Kollaboration & Kommunikation.
*   Gesteigerte Effizienz & Produktivität (Automatisierung).

## Auswahl & Implementierung von DevOps-Tools

**Faktoren bei der Auswahl:**
*   Organisationsstruktur & Umgebung (Teamgröße, Skills, Workflows).
*   Spezifische Ziele & Bedürfnisse (Problemlösung, Automatisierungsfähigkeiten).
*   Integrationsfähigkeit (APIs, Plugins).
*   Skalierbarkeit & Flexibilität.
*   Kosten & Lizenzierung (Open-Source vs. Kommerziell).

**Best Practices bei der Implementierung:**
*   Klare DevOps-Strategie entwickeln & kommunizieren.
*   Effektives Training & Kommunikation anbieten.
*   Klein anfangen & schrittweise skalieren (MVP, Pilotprojekte).
*   Tool-Wildwuchs ("Tool Sprawl") vermeiden.
*   Sicherheit & Compliance von Anfang an integrieren.

**Häufige Herausforderungen:**
*   Kultureller Widerstand gegen Veränderungen.
*   Mangel an qualifiziertem Personal.
*   Komplexe Legacy-Systeme.
*   Sicherstellung von Sicherheit & Compliance.
*   Management von Tool-Wildwuchs.

## DevOps Tool-Kategorien & Beispiele

### 1. Infrastructure Frameworks & Management Tools

*   **env0:** Kollaborative Plattform für IaC-Workflows (Terraform, OpenTofu, Pulumi etc.), Fokus auf Governance, Kostenkontrolle, RBAC, GitOps.
*   **Terraform (HashiCorp):** Deklarative IaC (HCL), Multi-Cloud, State Management, Module.
*   **Pulumi:** IaC mit gängigen Programmiersprachen (Python, JS, Go, .NET etc.), flexibel.
*   **OpenTofu:** Open-Source Fork von Terraform (kompatibel bis v1.5.6), Community-getrieben, neue Features (State Encryption).
*   **AWS CloudFormation:** Nativer AWS IaC-Dienst (JSON/YAML), tiefe AWS-Integration.

### 2. Version Control Systems (Plattformen)

*   **GitHub:** Populärste Git-Hosting-Plattform, Collaboration, Issues, GitHub Actions (CI/CD), Codespaces.
*   **GitLab:** All-in-One DevOps-Plattform, integriertes CI/CD, Issue Tracking, Container Registry.
*   **Bitbucket (Atlassian):** Git-Hosting, starke Integration mit Jira/Trello, Bitbucket Pipelines (CI/CD).

### 3. Configuration Management

*   **Ansible:** Agentenlos, einfache YAML-Syntax (Playbooks), große Modulbibliothek.
*   **Chef:** Ruby-basierte "Recipes", deklarativ, gut für große Umgebungen, Cookbooks.
*   **Puppet:** Deklarative DSL, Master-Agent-Architektur, Module, gut für Compliance.

### 4. Continuous Integration & Delivery (CI/CD)

*   **Jenkins:** Open-Source-Standard, riesiges Plugin-Ökosystem, flexibel, erweiterbar.
*   **CircleCI:** Cloud-basiert, containerisierte Builds, schnelle parallele Tests, gute Git-Integration.
*   **Spinnaker:** Open-Source, Multi-Cloud CD-Plattform, Deployment-Strategien (Canary, Blue/Green), Kubernetes-Integration.

### 5. Container Orchestration

*   **Kubernetes (K8s):** De-facto-Standard, Automatisierung von Deployment, Skalierung, Management containerisierter Apps, Self-Healing.
*   **Docker Swarm:** Native Docker-Clusterlösung, einfacher als K8s, gut für kleinere Setups.
*   **Nomad (HashiCorp):** Leichtgewichtiger Orchestrator für Container *und* Non-Container-Workloads (VMs, Batch), flexibel, Single Binary.

### 6. Security

*   **Checkov:** Statische Code-Analyse für IaC (Terraform, K8s, CloudFormation etc.), findet Fehlkonfigurationen.
*   **Snyk:** Developer-First-Security, scannt Code, Abhängigkeiten, Container, IaC auf Schwachstellen, IDE-Integration.
*   **Trivy:** Open-Source Scanner für Container-Images, Dateisysteme, Git-Repos auf Schwachstellen.

### 7. Cost Optimization

*   **Infracost:** Kostenabschätzung für IaC (Terraform), Integration in CI/CD, Cloud-Provider-Analyse (AWS, Azure, GCP).
*   **Kubecost:** Kostenoptimierung & -transparenz speziell für Kubernetes-Umgebungen.
*   **AWS Cost Explorer:** Natives AWS-Tool zur Visualisierung & Verwaltung von AWS-Kosten, Budgeting, Forecasting.

### 8. Monitoring & Observability

*   **Prometheus:** Open-Source Monitoring & Alerting, Time-Series-DB, PromQL, Pull-Modell, gut für K8s.
*   **Grafana:** Open-Source Visualisierungsplattform, Dashboards für diverse Datenquellen (Prometheus, etc.), Alerting.
*   **Datadog:** SaaS Monitoring & Analytics, Full-Stack Observability (Infra, Apps, Logs), viele Integrationen.
*   **New Relic:** SaaS Observability-Plattform, APM, Distributed Tracing, Log Aggregation, AI-Assisted Analysis.

## Wichtige FAQs

*   **Was ist ein DevOps-Tool?** Software, die Kollaboration, Automatisierung, Integration & Kommunikation zwischen Dev & Ops unterstützt.
*   **Bestes DevOps-Tool?** Man braucht meist *mehrere*. Beliebt: Terraform (IaC), Jenkins (CI/CD), Kubernetes (Orchestrierung).
*   **Ist Jira ein DevOps-Tool?** Primär Projektmanagement, aber integriert sich oft in DevOps-Workflows.
*   **Terraform vs. Pulumi?** Terraform nutzt HCL (DSL), Pulumi nutzt Programmiersprachen. Pulumi flexibler für komplexe Logik, Terraform einfacher & weiter verbreitet.
*   **Prometheus & Grafana?** Prometheus sammelt Metriken, Grafana visualisiert sie in Dashboards.
