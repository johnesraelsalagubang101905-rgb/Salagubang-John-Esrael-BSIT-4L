# Google Cloud Platform (GCP) - Reference Sheet

## Brief Overview
Google Cloud Platform (GCP) is Google's cloud computing platform. Instead of buying physical servers, companies rent Google’s high-speed computing infrastructure to run software, store data, and analyze massive amounts of information over the internet.

---

## Global Infrastructure
* **Regions:** Geographic areas around the world housing clusters of data centers. Picking a nearby region keeps apps running fast for local users.
* **Zones:** Distinct, fault-tolerant locations within a region. Deploying apps across multiple zones protects against hardware outages.
* **Private Fiber Network:** Google runs one of the world's largest private subsea fiber-optic networks, ensuring low-latency data speeds between data centers.

---

## Management Tools
* **Google Cloud Console:** A web-based dashboard used to configure, monitor, and control cloud resources visually.
* **gcloud CLI:** A command-line interface that allows developers to manage services using terminal commands and automated scripts.
* **Google Cloud Deployment Manager / Terraform:** Tools that let teams define their entire cloud setup as code for fast, repeatable deployments.

---

## Core Services

| Service | Category | Easy Analogy | What It Actually Does |
| :--- | :--- | :--- | :--- |
| **Compute Engine** | Compute | Rented virtual computer | Runs virtual machines (VMs) with custom CPU and RAM configurations on-demand. |
| **Cloud Storage** | Storage | Digital storage warehouse | Stores unstructured data (photos, media, backups, data logs) with multi-region backup. |
| **Virtual Private Cloud (VPC)** | Networking | Private virtual room | Connects your cloud resources inside a secure, private network isolated from the web. |
| **Cloud IAM** | Security | Security guard with a clipboard | Controls who has permission to access or modify specific Google Cloud resources. |
| **Google Kubernetes Engine (GKE)** | Containers | Traffic coordinator for app containers | Automatically manages and scales containerized applications (Docker). |
| **BigQuery** | Analytics | High-speed data engine | Analyzes terabytes or petabytes of data using SQL queries in seconds. |

---

## Key Advantages
* **Industry-Leading AI & ML:** Native access to Google's advanced machine learning models (Gemini, Vertex AI).
* **Kubernetes Pioneer:** Created by Google, making GCP the best environment for containerized app management.
* **Blazing Fast Global Network:** Uses Google's private backbone network rather than relying purely on public internet routing.
* **Smarter Big Data Tools:** Tools like BigQuery allow instant, serverless analysis of massive datasets without hardware setup.

---

## Common Enterprise Use Cases
* **AI & Machine Learning Companies:** Training custom models and running intelligent applications at scale.
* **Big Data & Analytics:** Analyzing millions of customer data points in real-time to drive business decisions.
* **High-Traffic Web & Mobile Apps:** Running scalable backends for streaming services, games, and consumer apps.
