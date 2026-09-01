# Checkpoint 4: Cloud Platform Recommendation Challenge

## CloudNova Technologies has received requests from four clients.

## Analyze each scenario and recommend the most appropriate cloud platform.

## Client A – Startup Company

### Recommended Cloud Platform
**Amazon Web Services (AWS)**

### Rationale
AWS is the ideal platform for a budget-conscious startup because its expansive pay-as-you-go pricing model and serverless architecture eliminate heavy upfront infrastructure costs. The platform provides access to programs like AWS Activate, which offers promotional credits that help early-stage companies minimize cash burn while developing their product. As the mobile application gains traction, AWS’s mature elastic scaling capabilities ensure the application smoothly scales from hundreds to millions of active users without architectural overhauls.

### Key AWS Services
* **AWS Amplify:** A comprehensive development framework that drastically accelerates mobile backend setup, automated builds, and frontend hosting.
* **Amazon Cognito:** Manages user registration, secure authentication, and social identity federation at scale with low pay-per-user costs.
* **AWS Lambda:** A serverless compute service that runs application code in response to mobile API requests, ensuring the client only pays for exact computing execution time.

---

## Client B – University

### Recommended Cloud Platform
**Microsoft Azure**

### Rationale
Microsoft Azure is the most practical choice for this university because it natively integrates with their existing Windows Server, Active Directory, and Microsoft 365 investments. By using Azure Hybrid Benefit, the university can reuse its existing Windows Server licenses to unlock substantial cost discounts on cloud virtual machines. Additionally, Microsoft Entra Connect enables effortless hybrid identity synchronization, allowing students, faculty, and administrative staff to access cloud resources using their current Active Directory credentials.

### Key Azure Services
* **Microsoft Entra ID (formerly Azure Active Directory):** Connects on-premises Active Directory accounts with cloud applications to deliver seamless Single Sign-On (SSO) and unified access management.
* **Azure Virtual Machines:** Allows IT staff to lift-and-shift existing Windows Server applications into managed, reliable cloud environments without rewriting code.
* **Azure Migrate:** Provides automated discovery and assessment tools to safely plan and execute the migration of university databases, web portals, and server workloads.

---

## Client C – AI Research Company

### Recommended Cloud Platform
**Google Cloud Platform (GCP)**

### Rationale
Google Cloud Platform is the premier environment for AI and machine learning workloads due to its native integration with cutting-edge AI frameworks and specialized hardware infrastructure. GCP provides direct access to custom Tensor Processing Units (TPUs) alongside high-performance GPU clusters, dramatically reducing the time required to train complex deep learning models. Supported by Google’s ultra-fast private fiber-optic network and industry-leading Big Data tools, data science teams can process petabyte-scale datasets with minimal latency.

### Key GCP Services
* **Vertex AI:** A unified machine learning platform that streamlines training, tuning, evaluating, and deploying custom AI models and Large Language Models (LLMs).
* **Google Kubernetes Engine (GKE):** The market's most advanced managed Kubernetes service, ideal for orchestrating scalable containerized AI pipelines and microservices.
* **BigQuery:** A serverless, highly scalable cloud data warehouse that executes lightning-fast SQL queries across massive research datasets in seconds.

---

## Client D – Global E-Commerce Company

### Recommended Cloud Platform
**Amazon Web Services (AWS)**

### Rationale
AWS is the industry leader for global e-commerce enterprise infrastructure due to its unmatched global presence, reliability, and auto-scaling performance during massive traffic surges. Its extensive network of Availability Zones and edge locations ensures that shopping pages load with low latency for customers anywhere in the world. Furthermore, AWS provides built-in compliance frameworks and high-throughput database systems designed to maintain 99.999% availability during high-volume sales events like Black Friday.

### Key AWS Services
* **Amazon CloudFront:** A global Content Delivery Network (CDN) that caches product imagery, media files, and static assets close to international shoppers for fast page loads.
* **Amazon DynamoDB:** A fully managed, multi-region NoSQL database that offers single-digit millisecond performance at any scale to support dynamic product catalogs and shopping carts.
* **Elastic Load Balancing (ELB) & Auto Scaling:** Automatically monitors web traffic and scales EC2 capacity up or down dynamically to prevent site crashes during unpredictable traffic spikes.








# Checkpoint 6: Multi-Cloud Decision Matrix

---

## 📊 Business Requirement Decision Matrix

| Business Requirement | Recommended Platform | Justification |
| :--- | :--- | :--- |
| **Startup Company** | 🟧 **AWS** | Offers a mature serverless ecosystem (AWS Amplify, Lambda) that minimizes upfront capital expenditure, combined with generous startup credit programs (AWS Activate) for fast MVP deployment. |
| **Enterprise Organization** | 🟧 **AWS** | Features the largest global infrastructure footprint, deepest service catalog (200+ services), highest compliance certifications, and the most expansive partner ecosystem in the market. |
| **Microsoft Environment** | 🟦 **Azure** | Delivers native, out-of-the-box integration with Windows Server, Active Directory, and Office 365, allowing companies to reuse software licenses via Azure Hybrid Benefit for massive cost savings. |
| **AI / Machine Learning** | 🟥 **GCP** | Provides industry-leading AI infrastructure (Vertex AI), custom TPU hardware acceleration, and advanced serverless data analytics (BigQuery) built on decades of Google AI research. |
| **Kubernetes Deployment** | 🟥 **GCP** | Google originally created Kubernetes; **Google Kubernetes Engine (GKE)** remains the premier, most mature managed container environment with seamless auto-scaling and minimal operational overhead. |
| **Global Web Application** | 🟧 **AWS** | Leverages a massive network of global Availability Zones, Elastic Load Balancing, and Amazon CloudFront (CDN) to deliver ultra-low latency and 99.999% availability during traffic surges. |

---

## 💡 Architectural Summary & Recommendations

* **Choose AWS if:** Your priority is maximum service selection, global reach, proven reliability under high-volume traffic, or building scalable cloud-native web and mobile applications from scratch.
* **Choose Azure if:** Your business heavily relies on existing Microsoft enterprise software, requires strong hybrid-cloud capabilities, or wants to optimize infrastructure costs via existing Windows/SQL licenses.
* **Choose GCP if:** Your applications center on data engineering, real-time analytics, machine learning model training, or heavily containerized microservices managed via Kubernetes.
