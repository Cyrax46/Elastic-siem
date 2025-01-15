# Elastic siem

## Objective

This project was aimed to establish a controlled environment for simulating and detecting cyber attacks. The primary focus was to ingest and analyze logs within a Security Information and Event Management (SIEM) system, generating test telemetry to mimic real-world attack scenarios. This hands-on experience was designed to deepen understanding of network security, attack patterns, and defensive strategies.

### Skills Learned

- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- Security Information and Event Management (SIEM) system for log ingestion and analysis(Elastic).
- Network analysis tool nmap,for capturing and examining network traffic.

## Steps
- Set up a free Elastic account.
- Install the Kali VM.
- Configure the Elastic Agent on the Linux VM to collect the logs and forward it to the SIEM.
- Generate security events on the Kali VM.
- Query to find the security events in the Elastic SIEM.
- Create a Dashboard to visualize security events.
- Create alerts for security events.

## Walkthough
- Step 1: Set up an Elastic Account
  
- Step 2: Setting up the Linux VM
  
- Step 3: Setting up the Agent to Collect Logs
  
 ![img-alt](https://github.com/Cyrax46/Elastic-siem/blob/bf0d4bb03c96887183a71d13e080085496dc528f/elastic%201.png)
 
 ![Elastic 1 5](https://github.com/user-attachments/assets/7243df98-d79a-43c3-9262-1c13dcad0dbb)
 
- Step 4: Paste this command into your kali terminal
  
 ![Elastic 2](https://github.com/user-attachments/assets/1ad7633d-5ade-49ec-8d1b-575c093e452c)

 ![Elastic 2 5](https://github.com/user-attachments/assets/72d598b9-96ff-45e5-80e1-b9c9f503b2e0)
- Step 5: Once the agent is installed we try to generate traffic in our kali machine.
  
 ![elastic 3](https://github.com/user-attachments/assets/c2fa9d87-c2d3-4cff-941b-b3b12dbf7df8)
- Step 6: Querying for Security Events in the Elastic SIEM
  
 ![Elastic 4](https://github.com/user-attachments/assets/e72dc722-864d-4e8a-a758-9912fbbafbbb)
 
- Step 7: We check for the nmap scans that we ran on our kali machine.
 ![Elastic 5](https://github.com/user-attachments/assets/413cbdee-4b82-4464-a495-41f7085306c2)

- Step 8: Create a Dashboard to Visualize the Events.
  
![Elastic 6](https://github.com/user-attachments/assets/ffb6efe0-89ee-4eee-a813-6494fb7249b2)

- Step 9: Click on the “Create dashboard” button on the top right to create a new dashboard.
  
- Step 10: Click on the “Create Visualization” button to add a new visualization to the dashboard.
  
- Step 11: Select “Area” or “Line” as the visualization type, depending on your preference.This will create a chart that shows the count of events over time.
  
 ![Elastic 7](https://github.com/user-attachments/assets/da902f9b-9872-4dc8-b3fe-b6a3bd0af6c7)
 
- Step 12: Click on the “Save” button to save the visualization and then complete the rest of the settings.
  
![Elastic 8](https://github.com/user-attachments/assets/69e8c3a9-95e2-4418-837c-0b3cdf3054a3)

- Step 13: Create an Alert
  
![Elastic 9](https://github.com/user-attachments/assets/323353a6-b0a8-494e-931c-d3f788a8439a)

- Step 14: Click on the “Create new rule” button at the top right.
  
- Step 15: Under the “Define rule” section, select the “Custom query” option from the dropdown menu
  
- Step 16: Under “Custom query,” set the conditions for the rule. You can use the following query to detect Nmap scan events.
  
- Step 17: This query will match all events with the action “nmap_scan.” Then click “Continue.”
  
- Step 18: Under the “About rule” section, give your rule a name and a description (Nmap Scan Detection).
  
- Step 19: Set the severity level for the alert, which can help you prioritize alerts based on their importance. Keep all the other default settings under “Schedule 
  rule” and click “Continue.”
  
![Elastic 10](https://github.com/user-attachments/assets/51394b51-0736-4004-802f-fb99c82bc3ce)

- Step 20: In the “Actions” section, select the action you want to take when the rule is triggered. You can choose to send an email notification, create a Slack 
  message, or trigger a custom webhook.
  
- step 21: Finally, click the “Create and enable rule” button to create the alert.





  
