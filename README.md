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

### Create resource group
<img width="1599" height="403" alt="z" src="https://github.com/user-attachments/assets/70c40169-bbb1-4120-a934-06ff1247c75f" />

- Chose Ubuntu Server because it’s lightweight, stable, and fully compatible with T-Pot’s Linux-based framework. It provides strong security, easy package management, and reliable performance

### Install PuTTY

<img width="1079" height="907" alt="x" src="https://github.com/user-attachments/assets/4eaee46d-7b3f-4f32-a116-24ce76ea13b3" />

- Installed PuTTY to securely connect to the Azure VM using SSH. It lets me access the Ubuntu server’s command line from Windows, so I can install and manage T-Pot remotely.

### Install T-Pot Multi Honeypot Git Package
https://github.com/telekom-security/tpotce
<img width="1055" height="999" alt="y" src="https://github.com/user-attachments/assets/23730c31-3dae-4438-97d1-e51fdde63e9b" />

### Go to the HTTPS https://20.106.16.132:64297/
<img width="1685" height="991" alt="1" src="https://github.com/user-attachments/assets/84464cdc-ee86-4071-a255-2a46cac7585e" />

### Explore Attack Map
<img width="1701" height="1062" alt="2" src="https://github.com/user-attachments/assets/13836638-01b3-4d5b-8e0d-b607c1ab6cf8" />

- Displays **live global attacker connections** targeting the honeypot.  
- **Arcs** show attack paths from source IPs to the honeypot’s location.  
- **Colored dots** represent attacker origins by protocol (FTP, SSH, HTTP, etc.).  
- **Tables below** list attack details — IP, country, service, and timestamp.  
- Provides a **real-time visualization** of global threat activity and attack trends.

### Explore Spiderfoot
<img width="1594" height="992" alt="12" src="https://github.com/user-attachments/assets/b6220c2e-5093-401d-b975-2790e8320890" />
<img width="1189" height="779" alt="13" src="https://github.com/user-attachments/assets/02c13049-2293-4d6c-b547-96fb44cb3099" />

- **Automated OSINT tool** used to gather intelligence on attacker IPs and domains.  
- Performs **reconnaissance and enrichment** using dozens of public data sources.  
- Reveals details such as **WHOIS info, geolocation, ASN, and threat reputation**.  
- Helps identify whether attacker IPs are from **known malicious networks or botnets**.  
- Enhances overall **threat analysis and attribution** in the honeypot project.

<img width="1196" height="310" alt="14" src="https://github.com/user-attachments/assets/47a82d5a-9ec7-4dc3-8895-b08016fd07a3" />

- Discover physical location where an IP is located with a scan

### Elastic Kibana Dashboard
<img width="1696" height="894" alt="i" src="https://github.com/user-attachments/assets/1338357b-8c7a-44f5-8b99-fdc7112cab9b" />

<img width="1688" height="564" alt="o" src="https://github.com/user-attachments/assets/6b13df68-dbaf-41e7-8798-770bb6aab5bd" />

- **Web interface** for visualizing and analyzing data collected by the honeypot.  
- Displays **dashboards, charts, and attack maps** built from Elasticsearch data.  
- Enables filtering by **timestamp, IP, country, and honeypot type** for deep analysis.  
- Provides **real-time insights** into attack volume, patterns, and sources.  
- Serves as the **main monitoring and visualization tool** for the T-Pot environment.  


## 🧾 TL;DR
Deployed **T-Pot**, a multi-honeypot framework, on **Microsoft Azure** to capture and analyze real-world cyberattacks.  
Integrated **Elastic Stack (Kibana, Logstash, Elasticsearch)** for live dashboards, **Attack Map** for visualization, and **SpiderFoot** for OSINT enrichment.  
This project demonstrates practical skills in **cloud security, threat detection, SIEM integration, and incident analysis**.





