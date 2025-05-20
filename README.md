# 📊 Monitor Fabric Activity in the Monitoring Hub

## 📌 Lab Objective

This lab focuses on using the **Monitoring Hub** in **Microsoft Fabric** to track the status and history of activities like dataflows and Spark notebooks. It demonstrates how to monitor, filter, and manage workloads in a Fabric workspace.

---

## 🛠️ Steps Performed

### 1. Create a Workspace
- Created a new **workspace** and ensured Fabric capacity was enabled (Trial, Premium, or Fabric).
- Verified that the workspace was created and empty.

---

### 2. Create a Lakehouse
- Selected **Create → Lakehouse** from the menu.
- Gave it a unique name.
- Confirmed that the **Lakehouse Explorer pane** appeared with no data.

---

### 3. Create and Monitor a Dataflow (Gen2)
- In the lakehouse homepage, selected **Get data → New Dataflow Gen2**.
- Named the dataflow: `Get Product Data`.
- Chose **Import from Text/CSV** and used this URL:  
  `https://raw.githubusercontent.com/MicrosoftLearning/dp-data/main/products.csv`
- Used **Anonymous authentication** to connect and preview data.
- Published the dataflow.

📍**Monitoring Activity**:
- Navigated to **Monitor → Monitoring Hub**.
- Refreshed to see the dataflow marked as **In-progress**, then **Succeeded**.
- Verified that the `products` table was created under the **Tables** folder in the lakehouse.

---

### 4. Create and Monitor a Spark Notebook
- Created a **Notebook** from the **Create** menu.
- Renamed it to: `Query Products`.
- Added the previously created **lakehouse** as a data source.
- Located the `products` table and selected **Load data → Spark**.
- Executed the notebook using **Run all**, and observed query results.
- Stopped the Spark session after execution.

📍**Monitoring Activity**:
- Checked the **Monitoring Hub** and confirmed the Spark notebook activity was listed.

---

### 5. Monitor Historical Runs
- Re-ran the `Get Product Data` dataflow by selecting **Refresh now**.
- In the Monitoring Hub, opened **Historical runs** from the `...` menu.
- Selected **View detail** to explore run metadata.

---

### 6. Customize the Monitoring Hub View
- Applied filters to show only:
  - **Status:** Succeeded
  - **Item type:** Dataflow Gen2
- Customized columns using **Column Options**:
  - Activity name
  - Status
  - Item type
  - Start time
  - Submitted by
  - Location
  - End time
  - Duration
  - Refresh type

---

### 7. Clean Up Resources
- Deleted the workspace after completing the lab to avoid unnecessary resource usage.

---

## 📘 What I Learned

- Navigated the **Microsoft Fabric Monitoring Hub** to track activities.
- Created and monitored:
  - **Lakehouse**
  - **Dataflow Gen2**
  - **Spark Notebook**
- Viewed **historical run details** and activity metadata.
- Applied **filters and custom views** for better observability.
- Understood how to **manage workloads efficiently** using Fabric's built-in tools.

---

This lab provided a hands-on experience in observing, debugging, and maintaining Fabric workflows — an essential part of managing real-world data platforms.

---

## Screeshots


<img width="1422" alt="Screenshot 2025-05-20 at 14 04 06" src="https://github.com/user-attachments/assets/bae5d38c-664e-48eb-82d7-ca20c5c334f4" />

<img width="1091" alt="Screenshot 2025-05-20 at 14 05 17" src="https://github.com/user-attachments/assets/18f23df6-9dce-49cb-b30f-6a6040c1fac8" />

<img width="1245" alt="Screenshot 2025-05-20 at 14 05 54" src="https://github.com/user-attachments/assets/284d46de-7ed3-400a-921e-078f34609022" />

<img width="1389" alt="Screenshot 2025-05-20 at 14 06 22" src="https://github.com/user-attachments/assets/4d8b8367-78d6-45a3-aa96-e0fc9a9b9021" />

<img width="1433" alt="Screenshot 2025-05-20 at 14 06 36" src="https://github.com/user-attachments/assets/2e2ff5c0-02de-4508-a248-8b3f8c76eb23" />

<img width="1493" alt="Screenshot 2025-05-20 at 14 08 39" src="https://github.com/user-attachments/assets/9feaacf9-5557-4966-95b2-07d21e00febf" />

<img width="1503" alt="Screenshot 2025-05-20 at 14 10 13" src="https://github.com/user-attachments/assets/66e5f3f9-8480-4189-8417-715a56c5ab94" />

<img width="1197" alt="Screenshot 2025-05-20 at 14 10 58" src="https://github.com/user-attachments/assets/994146e4-546d-4c77-8bb3-3c29b4b34859" />

<img width="967" alt="Screenshot 2025-05-20 at 14 12 25" src="https://github.com/user-attachments/assets/eb0239df-df51-4637-a545-cde1a4f79bff" />

<img width="1290" alt="Screenshot 2025-05-20 at 14 15 23" src="https://github.com/user-attachments/assets/cb84b360-cbdf-407e-853b-a61973c243ec" />

<img width="1423" alt="Screenshot 2025-05-20 at 14 18 19" src="https://github.com/user-attachments/assets/a59c1b37-3a0c-450d-abd5-5a9e47611cdd" />

<img width="1410" alt="Screenshot 2025-05-20 at 14 18 42" src="https://github.com/user-attachments/assets/c4968317-f67e-495c-afb3-87a0d93fdaa3" />
