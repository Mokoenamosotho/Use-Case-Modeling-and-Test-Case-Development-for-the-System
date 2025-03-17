

# AI-Driven Automated Database Recovery System - Test Cases

## 📌 Test Case Table

| **Test Case ID** | **Requirement ID** | **Description** | **Steps** | **Expected Result** | **Actual Result** | **Status (Pass/Fail)** |
|------------------|--------------------|-----------------|-----------|---------------------|-------------------|------------------------|
| **TC-001** | FR-001 | Automated Backup Scheduling | 1. Configure backup schedule for every 24 hours. <br> 2. Wait for the scheduled backup. <br> 3. Check backup logs. | A new backup is created, and logs are generated. | TBD | TBD |
| **TC-002** | FR-002 | AI-Powered Failure Prediction | 1. Simulate a failure-prone condition. <br> 2. Wait for prediction from the system. <br> 3. Verify alert issuance. | System predicts failure with 95% accuracy and issues an alert 24 hours before failure. | TBD | TBD |
| **TC-003** | FR-003 | Automated Data Recovery | 1. Simulate database failure. <br> 2. Trigger automatic recovery. <br> 3. Measure recovery time and verify data integrity. | Recovery completes within 30 minutes with no data loss exceeding 1 hour. | TBD | TBD |
| **TC-004** | FR-004 | Anomaly Detection & Alerting | 1. Perform unauthorized access or abnormal query execution. <br> 2. Check alerting system. | Alert is generated within 5 minutes, and anomaly is logged. | TBD | TBD |
| **TC-005** | FR-005 | Manual Override for Recovery | 1. Log in as IT admin. <br> 2. Pause recovery process. <br> 3. Resume or cancel the recovery process. | System allows recovery to be paused and resumed manually, with logs generated. | TBD | TBD |
| **TC-006** | FR-006 | Data Encryption for Backup & Recovery | 1. Trigger a backup operation. <br> 2. Inspect the encryption of backup data. | Backup data is encrypted using AES-256 encryption. | TBD | TBD |
| **TC-007** | FR-007 | Real-Time Database Health Monitoring | 1. Log into the monitoring dashboard. <br> 2. View real-time health metrics (e.g., CPU, memory, storage). <br> 3. Check if alerts are triggered. | Health metrics are updated in real-time, and alerts are triggered when limits are exceeded. | TBD | TBD |
| **TC-008** | FR-008 | Audit Trails for Backup & Recovery | 1. Perform a backup and recovery operation. <br> 2. Generate an audit report. <br> 3. Check if logs are properly maintained. | Audit trail is generated with timestamps, user actions, and system events. | TBD | TBD |
| **TC-009** | NFR-001 | Performance Test – Recovery Time | 1. Simulate database failure under normal load. <br> 2. Trigger recovery and measure recovery time. | Recovery completes within the 30-minute RTO. | TBD | TBD |
| **TC-010** | NFR-002 | Security Test – Unauthorized Access | 1. Attempt to log in using invalid credentials. <br> 2. Try accessing admin functionalities without authorization. | Unauthorized access is denied, and the event is logged. | TBD | TBD |

---

## ✅ **Notes:**
- **TBD (To Be Determined)** placeholders are for test execution results.
- **Test cases can be updated** to include additional validation points.
- Ensure that all **test cases are executed** in an appropriate environment.

