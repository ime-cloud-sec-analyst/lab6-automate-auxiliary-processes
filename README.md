# lab6-automate-auxiliary-processes
Practical implementation of Lab 6 in the SOAR lab series. This project automates auxiliary team processes using Splunk Phantom SOAR, including file transfer, permission adjustments, error handling, and system logging on Amazon Linux EC2.
Lab 6: Automate Auxiliary Team Processes – Full Lab Report
1. Lab Title & Description

Lab 6: Automate Auxiliary Team Processes

This lab focused on automating manual security operations tasks that auxiliary teams like SOC L1 Analysts or IT Helpdesk often carry out manually. The aim was to reduce human workload and accelerate standard responses using SOAR, AWS services, and Linux scripting.

2. Objectives

- Automate SOAR installation and setup on Amazon Linux 2023.
- Integrate IAM, EC2, and Linux scripts to simulate auxiliary operations automation.
- Demonstrate task orchestration, service management, and privilege handling.
- Capture and document the 31-step execution process in screenshots.

3. Scope & Purpose

This lab simulates how auxiliary teams' repeated actions (e.g., restarting failed services, alert investigation, backup validation, and SOAR agent communication) can be automated in a secure and repeatable way. This includes provisioning infrastructure and using Linux-based commands.

4. Tools & Technologies Used

- AWS EC2 (Amazon Linux 2023)
- Terminal CLI & Bash scripts
- Splunk SOAR (6.4.1)
- SSH for remote access
- wget, tar, chmod, and systemctl (Linux commands)

5. Key Steps Executed (31 Steps Documented)

- Launch EC2 instance (Amazon Linux 2023, t2.medium)
- Set security groups with SSH access (port 22)
- Generate and download new key pair
- SSH login to the instance
- Install SOAR using wget and tar
- Extract and assign permissions to SOAR binary
- Execute installation script and handle required password prompt
- Configure SOAR server & access web interface
- Monitor services using systemctl, logs, and SOAR CLI
- Capture each major step using screenshots

6. Implementation Strategy

- Manual execution using command-line in EC2
- Focused on core security automation use cases
- Ensured each step was captured in a picture for documentation
- Emphasis on infrastructure readiness, SOAR deployment, and task validation

7. Limitations & Challenges

- Some root-level commands were restricted due to unprivileged SOAR deployment.
- Required password entry after certain commands caused delays.
- Instance permissions and security configurations had to be adjusted carefully.
- Long setup and install time due to SOAR package size (~2.5 GB).

8. Outcomes & Achievements

- Successfully provisioned EC2 and deployed SOAR in Amazon Linux.
- Automation workflows were partially simulated using command-line and SOAR control.
- Gained experience in cloud provisioning, Linux service automation, and SOAR deployment.

9. Suggested README.md Summary for GitHub

# Lab 6: Automate Auxiliary Team Processes

This lab demonstrates the automation of auxiliary team tasks using Splunk SOAR and AWS EC2.
## Tools Used: AWS, Linux, Splunk SOAR, Bash
## Steps: EC2 launch → SOAR install → service automation → screenshots


10. GitHub Structure (Optional)

/lab6-automate-auxiliary/
├── screenshots/
│   ├── step1-launch-ec2.png
│   ├── step2-ssh-login.png
│   ├── ...
├── README.md
├── soar-install-script.txt
├── systemctl-output.log

11. Author & Contribution

Dr. Ime Ben – AWS Cloud Engineer & Security Automation Trainee
Contributed in design, execution, documentation, and review of the full 31-step lab.

