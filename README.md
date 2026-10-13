# Julián Ascenzi Márquez

Backend developer focused on building reliable APIs and services with Java and Python.

I care about data consistency, meaningful tests, and systems that are easy to understand, operate, and extend. My projects combine backend development with reproducible delivery, observability, and applied machine learning.

---

## Currently

- Looking for my first backend developer role
- Open to junior / semi-senior positions
- Based in Buenos Aires, Argentina · Open to remote

---

## Skills

- **Languages & Frameworks:** Java 21, Spring Boot 4, Python, FastAPI
- **Frontend:** React, TypeScript
- **Data & Persistence:** PostgreSQL, Flyway, JPA / Hibernate, transactions, concurrency control
- **Security:** JWT, Spring Security, BCrypt
- **Testing:** JUnit 5, Mockito, pytest, Playwright
- **Delivery & Infrastructure:** Docker, Docker Compose, Kubernetes (kind), Helm, GitHub Actions, GHCR, Terraform
- **Observability:** Prometheus, Grafana, Micrometer, Alertmanager, SLI / SLOs
- **ML / Data:** scikit-learn, pandas, Jupyter

---

## Projects

### [StockFlow](https://github.com/JulianAscenzi/StockFlow)

Full-stack inventory and sales application for small businesses, with product and category management, stock movements, sales history, a daily dashboard, and JWT-based administrator authentication.

- **Data consistency:** transactional sales and stock updates, pessimistic locking to prevent overselling, persistent idempotency, and historical sale snapshots.
- **Testing:** 385 backend tests and 28 Playwright scenarios in the latest documented checkpoints, covering PostgreSQL integration, concurrency, rollback, and browser flows.
- **Reliability:** health probes, graceful shutdown, structured logs, Prometheus/Grafana dashboards, SLOs, error budgets, and recovery experiments in local Docker/Kubernetes environments.
- **Delivery:** GitHub Actions tests OCI images before publishing to GHCR with SBOM/provenance; Helm deployments use image digests.
- **Cloud design:** Terraform for AWS ECS Fargate, ALB, and RDS, with static validation and mock tests. AWS infrastructure has not been provisioned.

`Java 21` · `Spring Boot 4` · `React` · `TypeScript` · `PostgreSQL` · `Flyway` · `Docker` · `Kubernetes` · `Helm` · `Terraform`

[Architecture](https://github.com/JulianAscenzi/StockFlow/blob/main/docs/ARCHITECTURE.md) · [Test evidence and project status](https://github.com/JulianAscenzi/StockFlow/blob/main/docs/STATUS.md) · [Reliability experiments](https://github.com/JulianAscenzi/StockFlow/blob/main/docs/KUBERNETES.md)

### [Churn Prediction](https://github.com/JulianAscenzi/churnPrediction)

End-to-end machine learning project that predicts telecom customer churn using the Telco Customer Churn dataset, with a reproducible training/evaluation workflow and a FastAPI service for inference.

- **Training:** data cleaning, encoding and scaling, a stratified train/test split, and a Random Forest classifier with balanced class weights.
- **Evaluation:** accuracy, precision, recall, F1, and a confusion matrix to assess performance on imbalanced data.
- **Inference:** a saved model artifact bundles the preprocessing metadata needed to process new customers consistently.
- **API:** `POST /predict` returns a churn prediction and probability, with Pydantic input validation, a health endpoint, and interactive OpenAPI documentation.
- **Testing:** data-processing tests use small synthetic DataFrames and run without downloading the dataset.

`Python` · `scikit-learn` · `FastAPI` · `Pydantic` · `pandas` · `pytest` · `Jupyter`

---

## Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-JulianAscenzi-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/juli%C3%A1n-ascenzi-19435b320/)
