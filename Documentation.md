# AI-Driven Automated Database Recovery System

## Test and Use Case Document

# 1. Stakeholder Analysis Table

| **Stakeholder**    | **Role**        | **Responsibilities**                                    | **Concerns**                                        |
|--------------------|-----------------|---------------------------------------------------------|-----------------------------------------------------|
| **IT Team**         | Primary user    | Configure, monitor, and troubleshoot the system        | Ensuring uptime and performance                     |
| **Database Admins** | End-user        | Manage database backups and recovery                   | Data integrity, backup reliability                  |
| **System Admins**   | End-user        | Configure AI models and oversee security               | Security, system performance                        |
| **Hospital Staff**  | Secondary user  | Use the database application                           | Data privacy, fast recovery                        |
| **Compliance Officer** | Oversight     | Ensure data recovery complies with legal regulations   | Compliance with data protection regulations (e.g., POPIA) |
| **Patients**        | Indirect user   | Indirectly affected by database reliability            | Privacy and confidentiality of health data          |

2. Functional and Non-Functional Requirements
3. Use Case Diagram

%% Example Use Case Diagram using mermaid.js
graph LR
  IT[IT Team] --> UC1[Backup Scheduling]
  IT --> UC2[Monitor Recovery Process]
  DB[Database Admins] --> UC3[Manage Recovery Settings]
  SA[System Admins] --> UC4[Configure AI Model]
  Patient[Patients] --> UC5[Access Database Info]
  Compliance[Compliance Officer] --> UC6[Ensure Compliance]
  UC1 --> UC7[Automated Backup Process]
  UC2 --> UC8[Alert Generation]
  UC3 --> UC9[Override Recovery]
  UC4 --> UC10[Update AI Model]

4. Use Case Specifications
5. Test Case Table

# AI-Driven Automated Database Recovery System - Test Cases

## 📌 Test Case Table

| **Test Case ID** | **Requirement ID** | **Description** | **Steps** | **Expected Result** | **Actual Result** | **Status (Pass/Fail)** |
|------------------|--------------------|-----------------|-----------|---------------------|-------------------|------------------------|
| **TC-001** | FR-001 | Automated Backup Scheduling | 1. Configure backup schedule. <br> 2. Wait for backup time. <br> 3. Check logs. | Backup is created, and logs are generated. | TBD | TBD |
| **TC-002** | FR-002 | AI-Powered Failure Prediction | 1. Simulate failure-prone condition. <br> 2. Wait for alert. | Alert is issued 24 hours before failure with 95% accuracy. | TBD | TBD |
| **TC-003** | FR-003 | Automated Data Recovery | 1. Trigger database failure. <br> 2. Wait for recovery process. <br> 3. Verify recovery time. | Recovery is completed within 30 minutes with no data loss exceeding RPO of 1 hour. | TBD | TBD |
| **TC-004** | FR-004 | Anomaly Detection & Alerting | 1. Perform unauthorized access or abnormal query. <br> 2. Check alert response. | Alert generated within 5 minutes, anomaly logged. | TBD | TBD |
| **TC-005** | FR-005 | Manual Override for Recovery | 1. Log in as IT admin. <br> 2. Pause recovery process. <br> 3. Resume or cancel recovery. | Manual override works, and actions are logged. | TBD | TBD |
| **TC-006** | FR-006 | Data Encryption for Backup & Recovery | 1. Trigger backup. <br> 2. Inspect encryption. | Backup is encrypted using AES-256. | TBD | TBD |
| **TC-007** | NFR-001 | Performance Test – Recovery Time | 1. Simulate failure. <br> 2. Measure recovery time. | Recovery completes within 30 minutes. | TBD | TBD |
| **TC-008** | NFR-002 | Security Test – Unauthorized Access | 1. Attempt invalid login. <br> 2. Try to access admin features. | Unauthorized access is denied, and event is logged. | TBD | TBD |

