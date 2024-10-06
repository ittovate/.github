---
marp: true
theme: gaia
---

<style>
     :root {
        --color-foreground: #040303; /* Light gray for text */
        --color-background: #FFFFFF; /* Dark navy blue for the background */
    }
    h1 {
        text-align: center;
    }
    h2 {
        display: flex;
        justify-content: center; /* Center horizontally */
        align-items: center; /* Center vertically */
        height: 100%; /* Use full height of the slide */
        font-size: 3em;
    }
    section {
        padding-bottom: 50px;
        font-size: 1.5em; /* Adjust the font size here */
    }
</style>

# 🚀 Overview

[ittovate organization](https://github.com/ittovate)
- demo-otp-service
- demo-db-to-kafka-to-db
- demo-mongo-crud
- demo-redis-crud
- demo-cassandra-crud
- demo-batch-processing
- demo-email-sender
- demo-email-listener
- demo-kafka
- demo-stripe-manager
- demo-chatbot

--- 

# 🎯 Learning Outcomes
- Standardize logging and exception handling
- Apply code quality checks using Checkstyle, SonarLint, and pre-commit hooks
- Manage application secrets securely
- Add unit and integration tests
- Write clear and comprehensive documentation
- Use CI workflow pipelines for automation
- Navigate technical documentation efficiently
- Implement authentication and authorization

---

# ⚠️ Challenges
- Redundancy copy/paste in multiple places **This led to thinking of packaging the most reusable parts as a separate module.**
- Apply Git & GitHub best practices.
- **demo-otp-service:** 
  - Choosing between RedisTemplate vs. Spring Data Redis had issues with expiration [Salesforce faced a similar issue](https://engineering.salesforce.com/lessons-learned-using-spring-data-redis-f3121f89bff9/)
- **demo-batch-processing:** 
  - **Challenges with resuming jobs**, particularly with Spring Batch's design that prevents resuming jobs after successful completion.
- **demo-email-listener:** 
  - Integration with Google Cloud and Gmail API 
  - Using Spring Email IMAP protocol
---
- **demo-kafka:** 
  - Setting up Schema Registry
  - Creating Avro for Serialization/Deserialization
- **demo-stripe-manager:** 
  - Understanding payment gateway integration (Business Aspect)
- **demo-chatbot:** 
  - Instability of the Spring AI framework and dependency issues, as the framework is still in progress

#### Other minor challenges included:
- Library/package incompatibility and conflicting dependencies 
- Tutorial hell **Led to more focus on navigating documentation well.**

--- 

# 🛠️ Skills Overview (1/2)

| **Member**   | **Skills**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Andrew**   | Rancher, K3s, Openshift/OKD, EKS, AKS, Kubeadm, Kustomize, Helm Chart, AWS, Azure, Linode, Hetzner, NodeJS, Java, Go, Python (Scripting), Bash, PostgreSQL, AWS Aurora, CockroachDB, MongoDB, Redis, Minio, S3, RabbitMQ, Kafka, Proxmox, VMware ESXi, Ceph, ELK, Grafana, Datadog, Zabbix, GitLab, GitHub Actions, ArgoCD, FluxCD, Ansible, Terraform, Jira, Freshdesk, PagerDuty, Airflow, Postman, JMeter                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Sabry**    | AI, Large Language Models (LLMs), Python, C#, Computer Vision                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Abuelmgad**| Java, JavaScript, Spring Boot, Spring Reactive, Spring Security, Redis, Kafka, PostgreSQL, MongoDB, Cassandra, Unit Testing, Mock Testing, Docker, Git/GitHub, Integration, Debugging, C#, Express.js, Static Code Analysis, SonarLint, Angular, React, Flutter, MySQL, SQLite, GitHub Actions, Ngrok, Reverse Proxy, AOP, Webclient, Authentication, Authorization, OAuth, API Development (REST)                                                                                                              |

---

# 🛠️ Skills Overview (2/2)

| **Member**   | **Skills**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|--------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Mohanad**  | C/C++, Java, C#, Spring Boot, Spring Data, Spring Kafka, Spring Batch, AOP, JavaScript, TypeScript, Node.js, Express.js, Docker, Kafka, Git/GitHub, PostgreSQL, MySQL, MongoDB, Redis, Unit Testing, Ngrok                                                                                                                                                                                                                                                                                                                    |
| **Hussein**  | C++, Java, Relational Databases, MongoDB, Unit Testing, Kafka, Docker, HTML, CSS, Bootstrap                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Al-Deeb**  | C++, Java, JavaScript, Python, Spring, Node.js, Django, Relational Databases, MongoDB, Unit Testing, Documentation, Kafka, Docker, Git/GitHub, Problem Solving                                                                                                                                                                                                                                                                                                                                        |
---

## What is next? 👀