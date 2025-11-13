# 📘 Amazon Redshift Immersion Labs 
### *Hands-on Data Engineering Project*

This project is based on the **AWS Redshift Immersion Labs** workshop.  
It covers Redshift Serverless, ELT processes, COPY jobs, S3 event integrations, data sharing, and performance monitoring.

---

# 📌 Project Overview

The goal of this project was to gain real-world hands-on experience with **Amazon Redshift Serverless**, including:

- Table design and schema configuration  
- Loading data using COPY from S3 and local files  
- Automating ingestion using S3 event notifications  
- Creating COPY Jobs for ELT workflows  
- Creating and querying Materialized Views  
- Sharing data across Redshift consumers  
- Monitoring query performance and tuning  

---

# 🏗️ Architecture

This architecture includes:

- **Redshift Serverless** as the primary data warehouse  
- **Amazon S3** for raw file ingestion  
- **S3 Event Notifications** to automate ingestion  
- **COPY Jobs** for ELT  
- **Materialized Views** to speed up queries  
- **Data Sharing** for federated analytics  
- **Monitoring Tools** for performance tuning  

---

# 🟦 1. Environment Setup — CloudFormation

### **1.1 — CloudFormation Stack (Lab Start Page)**  
![title](screenshots/1-title.png)

### **1.2 — Creating the CloudFormation Stack**
![stack-creation](screenshots/2-create-stack.png)

### **1.3 — CloudFormation Stack Created Successfully**
![stack-complete](screenshots/3-stack-creation-complete.png)

---

# 🟦 2. Connect to Redshift Query Editor v2

### **Redshift Query Editor Connected Successfully**
![query-editor](screenshots/4-Query Editor v2 connected.png)

---

# 🟦 3. Table Design & Manual Data Loading

### **3.1 — Creating Tables**
![table-creation](screenshots/5-Table creation.png)

### **3.2 — Loading Data from S3 Using COPY**
![copy-s3](screenshots/6-Loading data from S3 with copy command.png)

### **3.3 — Loading Data from Local File**
![load-local](screenshots/7-Load data from local file.png)

### **3.4 — Successful Local Ingestion**
![local-success](screenshots/8-load from local file successful.png)

### **3.5 — Example of Column Mismatch Error**
![mismatch-error](screenshots/9-try to load table with mismatched column.png)

### **3.6 — Troubleshooting Data Load Issues**
![troubleshoot](screenshots/10-To troubleshoot any data load issues.png)

---

# 🟦 4. ELT Workflow & Continuous Data Loads

### **4.1 — ETL Workflow Overview**
![etl](screenshots/11-ETL Workflow.png)

### **4.2 — ELT Workflow Overview**
![elt](screenshots/12-ELT Workflow.png)

### **4.3 — Updating S3 Bucket Policy**
![bucket-policy](screenshots/13-change bucket policy for ELT.png)

### **4.4 — Redshift Resource Policies for S3 Event Integration**
![policy](screenshots/14-redshift resource policies for S3 event.png)

### **4.5 — Creating S3 Event Integration**
![event1](screenshots/15-Create S3 event integration.png)

### **4.6 — S3 Event Integration Completed**
![event2](screenshots/16-S3 event integration.png)

### **4.7 — Creating a Redshift COPY Job**
![copy-job](screenshots/17-Create COPY JOB.png)

---

# 🟦 5. Materialized Views

### **5.1 — Creating a Materialized View**
![mv-create](screenshots/18-Create Materialized View.png)

### **5.2 — Querying Data Using the MV**
![mv-query](screenshots/19-Query with MV.png)

---

# 🟦 6. Data Sharing Between Redshift Clusters

### **6.1 — Creating a Data Share**
![datashare](screenshots/20-Create Data Sharing.png)

### **6.2 — Creating Database from Data Share & Testing**
![share-test](screenshots/21-Create Database and test datashare.png)

### **6.3 — Creating Additional User & Granting Permissions**
![permissions](screenshots/22-Create a user and grant permissions.png)

---

# 🟦 7. Query Monitoring & Performance Tuning

### **7.1 — Monitoring Dashboards**
![mon1](screenshots/23-Query & Database Monitoring.png)  
![mon2](screenshots/24-Query & Database Monitoring2.png)  
![mon3](screenshots/25-Query & Database Monitoring3.png)  
![mon4](screenshots/26-Query & Database Monitoring4.png)  
![mon5](screenshots/27-Query & Database Monitoring5.png)  
![mon6](screenshots/29-Query & Database Monitoring6.png)

### **7.2 — Deep Dive: Query ID Analysis**
![qid1](screenshots/28-QueryID-815726.png)  
![qid2](screenshots/30-QueryID-815726 Monitoring.png)

---

# 🧹 Cleanup

To avoid unexpected charges:

1. Delete Redshift Serverless workgroup  
2. Delete CloudFormation stack  
3. Empty & delete S3 bucket  
4. Remove IAM roles (if manually created)  

---

# 🏁 Final Thoughts

This project significantly strengthened my understanding of:

- Redshift data loading strategies  
- ELT workflow automation  
- Serverless data warehousing design  
- Data sharing across analytics workloads  
- Redshift monitoring and performance tuning  

---

# 🎓 Skills Gained

✔️ COPY Command & bulk data ingestion  
✔️ Automated ELT with S3 Event Notifications  
✔️ COPY Jobs in Redshift Serverless  
✔️ Materialized Views for performance  
✔️ Data Sharing concepts  
✔️ Schema design & sorting/distribution keys  
✔️ Query performance monitoring  
✔️ IAM & S3 integration  
✔️ Redshift Serverless workflow experience  
