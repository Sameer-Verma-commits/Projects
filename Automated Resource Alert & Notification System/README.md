To develop an automated system that:
   On demand monitors system resources
   Detects abnormal or high usage
   Sends real-time email alerts to the support team
   Logs all alerts in the database

The project integrates multiple technologies, each serving a specific purpose:

1. Python Programming Language:
Python was chosen due to its readability, extensive libraries, and strong support for automation. Key modules used include:
  •	psutil – for reading system resource usage (CPU, RAM, Disk).
  •	smtplib – to send emails using Gmail SMTP protocol.
  •	email.message – for constructing rich email messages.
  •	mysql.connector – for storing and retrieving alert logs and contact info.
	
3. MySQL Database:
The MySQL database stores:
  •	Support team details (names, email IDs)
  •	Alert logs with timestamp, resource type, message
This enables record-keeping and auditing of system warnings.

4. SMTP (Simple Mail Transfer Protocol):
Used for sending automated alerts via:
  •	Gmail SMTP Server
  •	TLS encryption for secure transmission
	
5. System Monitoring Technology:
Using psutil, the system captures:
  •	CPU Utilization
  •	RAM Usage
  •	Disk Partition Status
Thresholds determine when an alert needs to be generated.
