
Use Case Specifications

1️⃣ Use Case: Schedule Automated Backups
- Actor: IT Administrator, Database System
- Description: The system automatically schedules and executes database backups at predefined intervals.
- Precondition: The database system is operational, and backup settings are configured.
- Postcondition: A new backup is created, and logs are updated.

- Basic Flow:
1. IT Admin configures backup settings (frequency, storage location).
2. The system schedules backups accordingly.
3. At the scheduled time, the system initiates the backup.
4. Upon completion, the system logs the success or failure.
5. IT Admin receives a notification.

Alternative Flow:
- Failure Scenario: If backup fails, an alert is sent to the IT Admin, and the system retries after 10 minutes.

2️⃣ Use Case: Predict Failures Using AI
- Actor: AI Model, IT Administrator
- Description: The AI model analyzes system metrics to predict potential database failures.
- Precondition: AI model has been trained on past failure data.
- Postcondition: If a failure is predicted, an alert is generated.
- Basic Flow:
1. AI Model continuously monitors system performance.
2. AI detects patterns indicating potential failure.
3. If probability exceeds 95%, the system generates an alert.
4. IT Admin receives notification and takes preventive action.

Alternative Flow:
- If prediction confidence is below the threshold, AI continues monitoring without alerting.

3️⃣ Use Case: Trigger Automated Recovery
- Actor: IT Administrator, Database System
- Description: If a database failure occurs, the system automatically initiates recovery from the latest valid backup.
- Precondition: A backup exists, and the system detects failure.
- Postcondition: Database is restored to the last available backup.

Basic Flow:
1. System detects a failure.
2. An automatic recovery process is initiated.
3. The database is restored using the most recent backup.
4. The system logs the recovery process.
5. IT Admin receives a status update.

Alternative Flow:
- If the latest backup is corrupt, the system attempts to use the previous backup.

4️⃣ Use Case: Monitor Database Health
- Actor: IT Administrator, Hospital Management
- Description: The system continuously monitors database health and provides real-time performance metrics.
- Precondition: The monitoring service is running.
- Postcondition: System health metrics are displayed on the dashboard.

Basic Flow:
1. The system collects performance metrics (CPU, memory, storage, query response times).
2. Metrics are displayed on a real-time dashboard.
3. Alerts are triggered if thresholds are exceeded.
4. IT Admin reviews and takes action if necessary.

Alternative Flow:
- If monitoring service is unavailable, a notification is sent to the IT Admin.

5️⃣ Use Case: Detect and Alert Anomalies
- Actor: AI Model, Security Officer
- Description: The system detects anomalies in database usage patterns and alerts the security team.
- Precondition: AI Model is actively monitoring the database.
- Postcondition: An alert is issued if an anomaly is detected.

Basic Flow:
1. AI Model analyzes database access patterns.
2. It detects anomalies (e.g., unauthorized access, abnormal query patterns).
3. If an anomaly is detected, an alert is sent to the Security Officer.
4. The system logs the anomaly.

Alternative Flow:
- If the anomaly is a false positive, the Security Officer can mark it as safe.

6️⃣ Use Case: Manually Override Recovery
- Actor: IT Administrator
- Description: Allows IT Admin to manually trigger, pause, or cancel the automated recovery process.
- Precondition: The system has detected a failure or recovery is in progress.
- Postcondition: Manual action is logged.

Basic Flow:
1. IT Admin logs into the system.
2. Admin selects Pause, Resume, or Cancel Recovery.
3. System executes the chosen action.
4. The decision is logged, and IT Admin receives confirmation.

Alternative Flow:
- If IT Admin cancels recovery, a manual intervention plan is required.

7️⃣ Use Case: Encrypt Backup & Recovery
- Actor: Security Officer, Database System
- Description: Ensures that all backup and recovery operations are encrypted to protect sensitive data.
- Precondition: Encryption settings are configured.
- Postcondition: All backup and recovery processes use AES-256 encryption.

Basic Flow:
1. Security Officer configures encryption settings.
2. When a backup is created, encryption is applied.
3. During recovery, the system decrypts data securely.
4. Logs are updated with encryption details.

Alternative Flow:
- If encryption keys are unavailable, system raises an alert.

8️⃣ Use Case: Generate Audit & Compliance Reports
- Actor: Compliance Auditor, Hospital Management
- Description: Generates reports on system backups, recoveries, and security measures for regulatory compliance.
- Precondition: System logs must be enabled.
- Postcondition: A compliance report is generated and stored.

Basic Flow:
1. Compliance Auditor logs into the system.
2. Auditor selects report parameters (e.g., backup history, recovery attempts, security alerts).
3. System generates a compliance report.
4. Auditor downloads or reviews the report.

Alternative Flow:
- If logs are missing, the system notifies IT Admin for investigation.

