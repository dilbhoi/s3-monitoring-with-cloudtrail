# 📊 Task 4 – Monitoring AWS S3 Access using CloudTrail & CloudWatch

## 📌 Objective
To monitor and track S3 bucket activity using AWS services:
- **CloudTrail** for logging API events like file uploads or reads.
- **CloudWatch Logs** for real-time event visibility and tracking.

This setup helps detect unusual access, debug usage, and audit all actions performed on the S3 bucket.

---

## 🔍 Architecture Overview


- Every access or operation on the S3 bucket is logged via CloudTrail.
- These logs are forwarded to a CloudWatch log group.
- Events like `GetObject`, `PutObject`, `ListBucket` can be monitored in near real-time.

---

## ✅ Work Completed

- ✅ Created a **CloudTrail trail** and linked it to CloudWatch Logs
- ✅ Configured **CloudWatch Log Group** `/cloudtrail/s3-monitoring`
- ✅ Triggered log events by accessing the S3-hosted frontend
- ✅ Verified logs in **Log Stream** (with `eventName`, `eventSource`, and `bucketName`)
- ✅ Screenshots captured for verification

---

## 📂 Deliverables

- ✅ CloudTrail trail setup confirmation
- ✅ CloudWatch log group and log stream entries
- ✅ Events showing S3 access (e.g., `GetObject`, `PutObject`)
- ✅ (Optional) CloudWatch Dashboard or Alarm setup

---

## 🛠️ Technologies Used

- **AWS S3**
- **AWS CloudTrail**
- **AWS CloudWatch Logs**

---

## 📸 Screenshots (Recommended)

> Upload screenshots of:
- CloudTrail trail config page
- CloudWatch log group `/cloudtrail/s3-monitoring`
- A sample expanded log event (`eventName`, `eventTime`, `sourceIPAddress`)

---

## ✍️ How to Test

1. Access the hosted S3 frontend page.
2. Check CloudWatch log group for new events.
3. Verify logs show `eventName: GetObject` or similar entries.

---

## 🙌 Author

**Dil Bhoi**  
Intern @ Cloud Computing  
DY Patil International University, Pune
