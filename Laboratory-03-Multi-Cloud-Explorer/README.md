# Checkpoint 7 – Continue Your Linux Investigation

# ☁️ Linux Server Cloud Migration Reference Guide

**Source Machine Specs:**
* **OS:** Ubuntu 24.04.4 LTS (Noble Numbat) - x86_64
* **Compute:** 1 vCPU (Intel Xeon E312xx / KVM Hypervisor)
* **Memory:** 2.0 GiB RAM (410 MiB used, 1.5 GiB available)
* **Storage:** ~20 GB Root Partition (`/dev/vda1` with 13 GB free)

---

## 📊 Equivalent Cloud Hosting Services

| Resource Component | 🟧 Amazon Web Services (AWS) | 🟦 Microsoft Azure | 🟥 Google Cloud Platform (GCP) |
| :--- | :--- | :--- | :--- |
| **Compute Service** | **Amazon EC2** | **Azure Virtual Machines** | **Compute Engine** |
| **Recommended Instance Size** | `t4g.small` (ARM) or `t3.small` (2 vCPU, 2 GiB RAM) | `B1s` or `B2s` (1–2 vCPU, 1–4 GiB RAM) | `e2-micro` or `e2-small` (2 vCPU, 1–2 GiB RAM) |
| **OS Support** | Ubuntu 24.04 LTS (Noble Numbat) AMI | Ubuntu 24.04 LTS Image | Ubuntu 24.04 LTS Image |
| **Block Storage (20GB Disk)** | **Amazon EBS** *(gp3 volume)* | **Azure Managed Disks** *(Standard/Premium SSD)* | **Persistent Disk** *(pd-balanced / pd-ssd)* |
| **Virtual Networking** | **Amazon VPC** | **Azure Virtual Network (VNet)** | **Virtual Private Cloud (VPC)** |
| **Recommended Migration Tool** | **AWS Application Migration Service (MGN)** | **Azure Migrate** | **Migrate for Compute Engine** |

---

## 🚀 Migration Strategy Options

### 1. Lift and Shift (Rehosting as Virtual Machines)
Transfer the system directly into an Infrastructure-as-a-Service (IaaS) virtual machine:
* **AWS:** Deploy an EC2 instance using a default Ubuntu 24.04 AMI and mount a 20GB General Purpose SSD (gp3) EBS volume.
* **Azure:** Provision a B-series burstable virtual machine connected to a managed OS disk.
* **GCP:** Launch an `e2-small` Compute Engine instance using GCP's public Ubuntu 24.04 image.

### 2. Modernization Alternatives
* **Serverless Containers:** If hosting a microservice, web server, or script, containerize the application using Docker and deploy to serverless platforms (**AWS Fargate**, **Azure Container Apps**, or **Google Cloud Run**) to eliminate OS-level maintenance.
* **Lightweight VPS Hosting:** For simple, flat-rate hosting without enterprise VPC complexity, use **AWS Lightsail**, which offers identical 1 vCPU / 2 GB RAM Linux bundles for ~$10/month.
