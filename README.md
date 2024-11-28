# AUTOMATED CLOUD ENDPOINT ISOLATION WITH AI-ENHANCED THREAT DETECTION

## Objective
To build an automation system that identifies and isolates cloud-based endpoints (e.g., virtual machines, containers) when it detects unusual or potentially harmful behavior using AI-powered threat detection.

The Automated Cloud Endpoint Isolation with AI-enhanced Threat Detection project aimed to create an environment where cloud endpoints can be monitored for potential threats and isolated automatically using security automation and AI technologies. The goal is to build a system that integrates AWS CloudWatch for monitoring, AWS Lambda for automated response, Wazuh for log management, and AWS SageMaker for AI-driven analysis of detected threats. The project simulates real-world security incidents and responds by isolating compromised endpoints to minimize damage.

This hands-on experience was designed to:

Enhance understanding of cloud security automation.
Apply AI to improve threat detection and response in a cloud environment.
Develop practical experience with cloud-native security tools.

## Visual Work Flow

![image](https://github.com/user-attachments/assets/d2bb3d1e-2536-4cb7-998f-f53798d39feb)

## Skills Learned


- **Understanding Cloud Security Tools**:
  Gained practical experience with AWS security tools such as CloudWatch, Lambda, and SageMaker.
- **Automation with AWS Lambda**: Learned to automate threat response actions, such as isolating endpoints based on AI-driven analysis.
- **AI for Threat Detection**: Applied machine learning models in AWS SageMaker to analyze logs and detect abnormal behavior that indicates a potential security threat.
- **Security Incident Response**: Enhanced understanding of how to manage and automate security responses within a cloud environment.
- **Endpoint Security**: Gained practical experience in managing and isolating cloud endpoints when they are suspected of being compromised.
- **Log Analysis and Monitoring**: Strengthened knowledge of monitoring cloud infrastructure, analyzing logs, and identifying indicators of compromise (IoC).

## Tools Used

- **AWS CloudWatch**: For cloud infrastructure monitoring and log management.
- **AWS Lambda**: To automate responses such as isolating compromised endpoints or triggering further actions.
- **Wazuh**: To aggregate, analyze, and visualize logs from different cloud services.
- **AWS SageMaker**: For AI-driven threat detection and anomaly identification.
- **AWS SNS (Simple Notification Service)**: For alerting security teams about isolated endpoints or detected threats.
- **Slack**: Integrated with AWS SNS to send real-time notifications to the security team.


## Steps
1. **Setup AWS CloudWatch for Monitoring**

      Configured AWS CloudWatch to monitor and collect logs from various AWS services such as EC2 and Lambda.

      _Description: Here we see the CloudWatch dashboard where logs from EC2 instances are aggregated for analysis._

2. **Configure Wazuh for Log Aggregation**

      Set up Wazuh to collect and parse logs from AWS CloudWatch, aggregating security-related events for further analysis.

      _Description: Wazuh configuration to ingest AWS CloudWatch logs for centralized security event management._

3. **Implement AWS Lambda for Automated Endpoint Isolation**

     Developed Lambda functions that automatically isolate compromised EC2 instances by modifying security groups when         specific threat signatures are detected.

      _Description: Lambda function that triggers when a potential threat is identified, isolating the affected endpoint._

4. **Develop AI Models in AWS SageMaker for Threat Detection**

      Used SageMaker to develop machine learning models that analyze logs and detect anomalous patterns indicative of a security breach.
   
     _Description: Screenshot of the SageMaker model training interface, where a machine learning model is trained to identify attack patterns._
5. **Integrate AWS SNS and Slack for Alerting**

    Configured AWS SNS to send real-time alerts when an endpoint is isolated. These alerts were then forwarded to a Slack channel for team visibility.

    _Description: SNS alert setup to notify the security team on Slack when an endpoint is automatically isolated._

6. **Test and Validate the System**

      Ran multiple test scenarios to simulate different types of cyberattacks, ensuring the automated system responds appropriately by isolating compromised endpoints.
   
   _Description: Logs from the test simulations showing how the system automatically isolates a compromised endpoint._


## Conclusion
   This project successfully demonstrated the integration of cloud-native security tools with AI to automate the detection and response to security incidents. 
   
   By automating endpoint isolation and leveraging machine learning for threat detection, the system offers an efficient and scalable way to protect cloud environments. 
   
   The challenge of balancing security automation with real-time responses was met, and this project is a step forward in enhancing cloud security operations.
