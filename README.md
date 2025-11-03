# T-Pot Honeypot Deployment & Threat Detection (Microsoft Azure)

<img width="1698" height="1065" alt="honey" src="https://github.com/user-attachments/assets/99c5e352-e1a7-46ee-b552-62c78983eec5" />


## 🎯 OBJECTIVE

The objective is to simulate and monitor active cyber threats in a controlled Azure environment by deploying the T-Pot honeypot suite. This project showcases hands-on experience with threat detection, incident response, and data enrichment using ELK dashboards and GeoIP mapping.


## 🔧 KEY TOOLS & TECHNOLOGIES
- **Microsoft Azure** – Cloud platform used to host and manage the virtual machine environment.  
- **T-Pot** – All-in-one **multi-honeypot framework** integrating multiple honeypot services for capturing diverse attack traffic.  
- **Elastic Stack (ELK: Elasticsearch, Logstash, Kibana)** – Centralized log collection, correlation, and real-time attack visualization.  
- **Attack Map (Kibana Visualization)** – Displays live global attacker IP activity with GeoIP-enriched data.  
- **Elasticvue** – Elasticsearch GUI extension used for exploring, querying, and managing indexed honeypot data.  
- **SpiderFoot** – Automated OSINT tool used for enrichment and investigation of attacker IPs and domains.  
- **Ubuntu Server** – Operating system used for the honeypot deployment.  
- **Docker** – Containerized environment to isolate and manage multiple honeypot services.  
- **GeoIP Database (MaxMind)** – Enriches attacker IPs with geographic and ASN data for location mapping.  
- **Kibana Dashboards** – Interactive visualizations to monitor attacks, protocols, and honeypot activity trends.  
- **SSH (PuTTY / Terminal)** – Secure remote access for deploying, configuring, and maintaining the honeypot system.  


## ⚙️ DEPLOYMENT
