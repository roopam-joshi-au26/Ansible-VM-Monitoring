This project provides an Ansible-based solution for monitoring the health of virtual machines (VMs) by collecting key system metrics such as CPU and memory usage. It enables administrators to proactively track resource utilization across multiple Linux-based VMs without the need for installing additional agents.

🔧 Features
Agentless Monitoring: Utilizes SSH to connect to target VMs, eliminating the need for agent installation.

Resource Utilization Metrics: Gathers real-time data on CPU and memory usage using native Linux commands.

Automated Reporting: Aggregates collected metrics and sends summary reports via email to designated recipients.

Scalable Architecture: Designed to monitor a large number of VMs efficiently from a central Ansible control node.

Customizable Alerts: Thresholds can be configured to trigger alerts when resource usage exceeds defined limits.

📁 Project Structure
Inventory File: Lists all target VMs to be monitored.

Playbooks: YAML files defining tasks for data collection and reporting.

Templates: Jinja2 templates for formatting email reports.

Scripts: Auxiliary scripts for setting up and managing the monitoring process.

🚀 Getting Started
Install Ansible: Ensure Ansible is installed on the control node.

Configure Inventory: Define the target VMs in the inventory file.

Customize Variables: Set thresholds and email configurations in the variables file.

Run Playbook: Execute the main playbook to start monitoring.

📬 Example Output
Upon execution, the system sends an email report summarizing the CPU and memory usage of each monitored VM, aiding in quick identification of potential issues. 
