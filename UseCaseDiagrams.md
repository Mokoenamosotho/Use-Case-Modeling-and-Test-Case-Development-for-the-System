Task 1: Use Case Diagrams 

Key Actors and Their Roles

1. IT Administrator 👨‍💻
- Manages system configurations.
- Oversees automated backups and database recovery.
- Monitors system health and manually intervenes when necessary.

2. Database System 💾
- Stores critical hospital data.
- Works with the backup and recovery system for data protection.

3. AI Model 🤖
- Predicts potential database failures based on historical data.
- Detects anomalies and security threats.

4. Compliance Auditor 📜
- Reviews backup and recovery logs for regulatory compliance.
- Ensures adherence to POPIA and hospital policies.

5. Hospital Management 🏥
- Oversees database health reports.
- Ensures smooth IT operations across departments.

6. Security Officer 🔒
- Ensures data encryption and cybersecurity measures are in place.
- Investigates anomalies and potential security threats.

Relationships Between Actors and Use Cases

- The IT Admin directly interacts with the backup, recovery, monitoring, and manual override features to maintain database reliability.
- The AI Model autonomously predicts failures and detects anomalies to improve database uptime.
- The Compliance Auditor requires access to audit logs for verifying legal compliance.
- The Security Officer ensures data encryption and anomaly detection, protecting sensitive patient information.
- Hospital Management mainly monitors system performance and reviews compliance reports to ensure efficiency.

Mermaid Use Case Diagram

graph TD
  %% Define actors
  IT_Admin["👨‍💻 IT Admin"]
  Database_System["💾 Database System"]
  AI_Model["🤖 AI Model"]
  Compliance_Auditor["📜 Compliance Auditor"]
  Hospital_Management["🏥 Hospital Management"]
  Security_Officer["🔒 Security Officer"]

  %% Define use cases
  UC1["Schedule Automated Backups"]
  UC2["Predict Failures Using AI"]
  UC3["Trigger Automated Recovery"]
  UC4["Monitor Database Health"]
  UC5["Detect and Alert Anomalies"]
  UC6["Manually Override Recovery"]
  UC7["Encrypt Backup & Recovery"]
  UC8["Audit & Compliance Reports"]
  UC9["Generate IT Reports"]

  %% Connect actors to use cases
  IT_Admin --> UC1
  IT_Admin --> UC3
  IT_Admin --> UC4
  IT_Admin --> UC6
  IT_Admin --> UC9

  Database_System --> UC1
  Database_System --> UC3
  Database_System --> UC4

  AI_Model --> UC2
  AI_Model --> UC5
  AI_Model --extends--> UC4  %% AI improves real-time monitoring

  Compliance_Auditor --> UC8

  Hospital_Management --> UC4
  Hospital_Management --> UC8
  Hospital_Management --> UC9

  Security_Officer --> UC5
  Security_Officer --> UC7
