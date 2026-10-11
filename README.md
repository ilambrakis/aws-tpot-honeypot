# AWS T-Pot Honeypot Deployment

## Objective

The goal of this project was to deploy a cloud-hosted T-Pot honeypot using AWS EC2 and Ubuntu Linux to gain hands-on experience with cloud infrastructure, Linux administration, AWS networking, SSH authentication, cybersecurity monitoring, and honeypot deployment.

This project was completed to develop practical skills commonly used in Security Operations Center (SOC) environments while learning how cloud-hosted security monitoring platforms are deployed and managed.

## Skills Learned

- AWS EC2 deployment and management
- Linux administration using Ubuntu
- SSH authentication and remote server access
- AWS Security Group configuration
- Cloud infrastructure management
- Cybersecurity monitoring concepts
- Honeypot deployment and configuration
- Docker container deployment
- Troubleshooting Linux and networking issues
- Technical documentation and project reporting

## Tools Used

- AWS EC2
- Ubuntu Linux
- Kali Linux
- T-Pot
- Kibana
- Elasticsearch
- Docker
- VirtualBox
- GitHub
- SSH

## Deployment Steps

### Phase 1: AWS Infrastructure Setup

1. Created an Ubuntu EC2 instance in AWS.
2. Generated a PEM key pair for SSH authentication.
3. Configured AWS Security Group inbound rules.
4. Prepared the cloud environment for T-Pot deployment.

**Ref 1: AWS EC2 Instance Deployment**

The AWS EC2 instance was successfully launched and entered a running state. This Ubuntu-based instance served as the host for the T-Pot honeypot environment.

<img width="2041" height="1213" alt="pic-1-instance-launched" src="https://github.com/user-attachments/assets/bf9cd543-d525-4176-a690-865b3037f27b" />

---

**Ref 2: Secure SSH Connection**

A secure SSH connection was established between the Kali Linux virtual machine and the AWS EC2 Ubuntu instance using a PEM key for authentication. This enabled remote administration and configuration of the Ubuntu server.

<img width="1729" height="1239" alt="pic 2" src="https://github.com/user-attachments/assets/45c808d3-f946-4e39-b22b-a0bccf3f3048" />

---

### Phase 2: T-Pot Installation

1. Connected to the Ubuntu server.
2. Cloned the official T-Pot repository.
3. Executed the installation script.
4. Configured the deployment environment.
5. Installed required monitoring and honeypot services.

**Ref 3: Preparing the Ubuntu Server for T-Pot Installation**

Administrative access was established on the Ubuntu EC2 instance. The official T-Pot repository was cloned from GitHub, and the installation script was launched to begin deployment of the honeypot environment.

<img width="1727" height="1242" alt="pic 3 installing tpot" src="https://github.com/user-attachments/assets/0f9efbfa-9113-4e77-be37-bbe56bd57b3b" />

---

**Ref 4: T-Pot Installation Configuration**

During installation, web interface credentials were configured and Docker images were downloaded. These images included Kibana, Elasticsearch, Cowrie, Honeytrap, and other services required for the T-Pot platform.

<img width="1730" height="1243" alt="pic 4 installed" src="https://github.com/user-attachments/assets/b427ae33-1430-4efd-b8e1-728c977a56d7" />

---

**Ref 5: T-Pot Installation Completed**

The T-Pot installation completed successfully and the web interface became accessible. This confirmed that deployment was successful and that integrated monitoring tools were available through the platform.

<img width="1709" height="1383" alt="pic 5 tpot" src="https://github.com/user-attachments/assets/b2c71322-987f-4768-9e65-f7cc08633ddb" />

---

### Phase 3: Dashboard Validation

**Ref 6: T-Pot Attack Map**

The Attack Map dashboard was successfully accessed through the T-Pot platform. This feature provides geographic visualization of traffic and activity collected by the honeypot environment.

<img width="1718" height="1439" alt="pic 6 attack map" src="https://github.com/user-attachments/assets/32f13848-2dd8-4bd5-a3d8-f2b1f73376be" />

---

**Ref 7: Kibana Dashboard**

Kibana was successfully accessed through the Elastic Stack deployment, providing centralized visualization and monitoring capabilities for collected security data.

<img width="1715" height="1437" alt="pic 7 kibana" src="https://github.com/user-attachments/assets/cbe3eb0f-58e0-47e3-a76f-9cba86ca0c6c" />

---

### Phase 4: Security Configuration

**Ref 8: AWS Security Group Configuration**

AWS Security Group rules were configured to permit management access and required honeypot services while maintaining appropriate network security controls.

<img width="1714" height="1311" alt="pic 8 inbound rules" src="https://github.com/user-attachments/assets/2067370d-6a7c-4750-9a80-25c81f5b7031" />

---

## 🧠 Key Takeaways

- Gained hands-on experience deploying and managing cloud infrastructure using AWS EC2.
- Strengthened Linux administration and command-line skills.
- Learned how SSH authentication is used in cloud environments.
- Developed practical experience configuring AWS Security Groups and network access controls.
- Successfully deployed and validated a cloud-hosted T-Pot honeypot environment.
- Improved troubleshooting skills involving AWS, Linux, Docker, and cybersecurity monitoring tools.
- Developed documentation skills by creating a structured deployment report and project portfolio.

## 🚀 Future Improvements

- Leave the honeypot deployed for a longer period to collect attack telemetry.
- Analyze attack data and identify common sources of malicious activity.
- Create Kibana visualizations based on collected attack data.
- Integrate additional monitoring and alerting capabilities.
- Expand the project into a larger home lab environment.
