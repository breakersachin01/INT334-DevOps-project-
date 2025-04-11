# Kubernetes Cluster Deployment and Static Website Monitoring Using Prometheus, Grafana, and Splunk

This project demonstrates the deployment of a Kubernetes cluster on AWS EC2 instances and showcases monitoring a static website using Prometheus, Grafana, and Splunk.

## 🚀 Project Highlights

- Deploy a Kubernetes master-slave cluster using kubeadm on AWS EC2
- Host a static website using an NGINX pod
- Monitor the cluster and website performance using:
  - Prometheus for metrics collection
  - Grafana for visualization
  - Splunk for log monitoring
- Services exposed via NodePort for browser-based access

---

## 🧰 Tech Stack

- Kubernetes (kubeadm)
- AWS EC2 (Ubuntu 20.04)
- NGINX (for static website)
- Prometheus (metrics)
- Grafana (dashboards)
- Splunk (log monitoring)
- Helm (for Prometheus Operator)

---

## 📂 Project Structure


---

## ⚙️ Setup Instructions

1. Launch two Ubuntu EC2 instances on AWS:
   - Master Node
   - Worker Node

2. Set up Kubernetes:
   - Initialize master node
   - Join worker node to cluster

3. Deploy static website:
   - Apply static-site.yaml and static-site-service.yaml

4. Deploy Prometheus and Grafana:
   - Install Helm
   - Deploy Prometheus Operator using Helm

5. Deploy Splunk in a pod:
   - Apply splunk-deployment.yaml and splunk-service.yaml

6. Access Services:
   - Static site: http://<NodeIP>:<NodePort>
   - Grafana: http://<NodeIP>:<GrafanaNodePort>
   - Splunk: http://<NodeIP>:<SplunkNodePort>

---

## 📈 Future Improvements

- Add Ingress controller with TLS
- Configure Alertmanager for Prometheus
- Enable CI/CD pipeline
- Add authentication for dashboards

---

## 🙋 Author

- 👨‍💻 Sachin Vishwakarma
- 📧 vishwakarmasachin632@gmail.com
