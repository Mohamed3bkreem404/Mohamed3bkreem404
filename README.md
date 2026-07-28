<p align="center">
  <img src="./assets/profile-banner.png" alt="Mohamed Abdelkareem — Cloud and Platform Engineering" width="100%" />
</p>

<h1 align="center">Mohamed Abdelkareem</h1>

<p align="center">
  <strong>Cloud & Platform Engineering</strong><br/>
  Kubernetes · Infrastructure as Code · GitOps · Observability
</p>

<p align="center">
  Junior DevOps Engineer and Computer Science student building production-style cloud platforms on AWS.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/mohamed-abdelkareem-311317357">LinkedIn</a>
  &nbsp;·&nbsp;
  <a href="mailto:mo.abdelkareem.ahmed@gmail.com">Email</a>
  &nbsp;·&nbsp;
  <a href="./assets/Mohamed_Abdelkareem_CV.pdf">Resume</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/Mohamed3bkreem404/International-Commerce">Flagship Project</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/AWS-0B0D10?style=flat-square&logo=amazonwebservices&logoColor=FF9900" alt="AWS" />
  <img src="https://img.shields.io/badge/Terraform-0B0D10?style=flat-square&logo=terraform&logoColor=844FBA" alt="Terraform" />
  <img src="https://img.shields.io/badge/Kubernetes-0B0D10?style=flat-square&logo=kubernetes&logoColor=326CE5" alt="Kubernetes" />
  <img src="https://img.shields.io/badge/Helm-0B0D10?style=flat-square&logo=helm&logoColor=0F1689" alt="Helm" />
  <img src="https://img.shields.io/badge/Argo_CD-0B0D10?style=flat-square&logo=argo&logoColor=EF7B4D" alt="Argo CD" />
  <img src="https://img.shields.io/badge/GitHub_Actions-0B0D10?style=flat-square&logo=githubactions&logoColor=2088FF" alt="GitHub Actions" />
  <img src="https://img.shields.io/badge/Prometheus-0B0D10?style=flat-square&logo=prometheus&logoColor=E6522C" alt="Prometheus" />
  <img src="https://img.shields.io/badge/Grafana-0B0D10?style=flat-square&logo=grafana&logoColor=F46800" alt="Grafana" />
</p>

Engineering profile

I work at the intersection of cloud infrastructure, delivery automation, and application reliability. My main project is a production-style commerce platform built around Spring Boot microservices and operated using AWS, Terraform, Docker, Kubernetes, Helm, Argo CD, GitHub Actions, Ansible, Prometheus, and Grafana.

I focus on systems that are:

Reproducible — infrastructure and platform configuration live in code.

Declarative — desired state is versioned, reviewed, and continuously reconciled.

Observable — metrics, dashboards, alerts, and health checks are part of the design.

Failure-aware — rollbacks, probes, resource limits, scaling, backups, and recovery paths are explicit.

Secure by default — least privilege, network isolation, TLS, secrets management, and access control are built in.

Platform capabilities

Layer

What I build and operate

Cloud

AWS VPC networking, public/private subnets, NAT, ALB, EC2, RDS, IAM, S3, DynamoDB, and CloudWatch

Infrastructure

Modular Terraform, remote state, Ansible automation, Bash and Python tooling, Linux administration

Containers

Multi-stage Docker builds, Docker Compose, Kubernetes Deployments and StatefulSets, Services, PVCs, probes, resource controls, and HPA

Delivery

GitHub Actions, image versioning, Helm releases, Argo CD synchronization, self-healing, pruning, and rollback workflows

Observability

Prometheus, Grafana, Alertmanager, Actuator, Micrometer, PostgreSQL Exporter, cAdvisor, and CloudWatch

Application context

Java, Spring Boot, REST APIs, OpenFeign, Next.js, TypeScript, PostgreSQL, Redis, JWT, and RBAC

Selected work

International Commerce — Cloud-Native E-Commerce Platform

A production-style platform composed of an API Gateway, five domain microservices, a Next.js frontend, service-owned PostgreSQL databases, Redis caching, automated cloud infrastructure, Kubernetes delivery, GitOps, and end-to-end observability.

<p>
  <a href="https://github.com/Mohamed3bkreem404/International-Commerce">
    <img src="https://img.shields.io/badge/View_repository-11151A?style=flat-square&logo=github&logoColor=white" alt="View repository" />
  </a>
</p>

Engineering outcomes

Result

Implementation

Under 12 minutes

Rebuilt the AWS environment using modular Terraform

More than 80% faster delivery

Reduced deployment time from about 20 minutes to under 4 minutes

About 60% smaller images

Reduced service images from roughly 800 MB to 320 MB with multi-stage builds

2 → 8 replicas

Configured HPA scaling at 70% CPU utilization

Protected Terraform state

Used an S3 remote backend with DynamoDB locking

Platform architecture

flowchart LR
    Engineer[Engineer] --> GitHub[GitHub]
    GitHub --> Actions[GitHub Actions]
    Actions --> Registry[Container Registry]
    Actions --> Config[Versioned Helm Values]
    Config --> Argo[Argo CD]
    Argo --> Cluster[Kubernetes Platform]
    Registry --> Cluster

    Client[Web Client] --> ALB[AWS ALB]
    ALB --> Edge[Traefik / Ingress]
    Edge --> Gateway[API Gateway]

    Gateway --> User[User Service]
    Gateway --> Product[Product Service]
    Gateway --> Cart[Cart Service]
    Gateway --> Order[Order Service]
    Gateway --> Payment[Payment Service]

    User --> RDS[(PostgreSQL)]
    Product --> RDS
    Cart --> RDS
    Order --> RDS
    Payment --> RDS
    Product --> Redis[(Redis)]

    Cluster -. metrics .-> Prometheus[Prometheus]
    Prometheus --> Grafana[Grafana]
    Prometheus --> Alertmanager[Alertmanager]
    Cluster -. infrastructure metrics .-> CloudWatch[CloudWatch]

What this project demonstrates

AWS networking and infrastructure provisioning with Terraform.

Container build optimization and repeatable local environments.

Kubernetes orchestration for stateful and stateless workloads.

Reusable Helm charts for application, monitoring, and GitOps resources.

Automated build, versioning, image publishing, deployment, and health validation.

GitOps synchronization with self-healing and pruning.

JVM, application, database, container, and infrastructure monitoring.

TLS, security headers, rate limiting, least-privilege IAM, JWT, and role-based access control.

TaskOps Platform — DevOps Practice Lab

A Spring Boot monolith used as an isolated engineering lab for Docker, CI/CD, infrastructure automation, and failure-driven operational practice.

<p>
  <a href="https://github.com/Mohamed3bkreem404/TaskOps-Platform">
    <img src="https://img.shields.io/badge/View_repository-11151A?style=flat-square&logo=github&logoColor=white" alt="View TaskOps repository" />
  </a>
</p>

The goal is not another application demo. It is a controlled place to test delivery workflows, break infrastructure safely, document failure modes, and turn fixes into repeatable automation.

Technical progression

Backend foundations
Java · Spring Boot · REST APIs · PostgreSQL · Redis
        ↓
Delivery and operations
Linux · Docker · GitHub Actions · Networking · Automation
        ↓
Cloud platform engineering
AWS · Terraform · Kubernetes · Helm · Argo CD · Ansible
        ↓
Reliability engineering
Prometheus · Grafana · Alertmanager · Health checks · Scaling · Recovery

Current focus

Making Terraform and Helm components easier to reuse across environments.

Improving GitOps promotion, rollback, drift visibility, and deployment safety.

Turning operational knowledge into architecture records, runbooks, and failure scenarios.

Strengthening platform security through policy, automated validation, and least-privilege design.

Expanding observability from dashboards into service-level signals and actionable alerts.

Open engineering

I use public repositories as engineering case studies: architecture, decisions, automation, trade-offs, failures, and recovery steps should be visible—not hidden behind a wall of technology logos.

Issues, reviews, and practical infrastructure discussions are welcome.

<p align="center">
  <strong>Open to Junior DevOps, Cloud, Platform, and Infrastructure Engineering opportunities.</strong>
</p>

<p align="center">
  <a href="mailto:mo.abdelkareem.ahmed@gmail.com">mo.abdelkareem.ahmed@gmail.com</a>
  &nbsp;·&nbsp;
  <a href="https://www.linkedin.com/in/mohamed-abdelkareem-311317357">LinkedIn</a>
</p>
