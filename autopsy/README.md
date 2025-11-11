# **Experiment 05: Forensic Investigation Using Autopsy**

## **Objective**
To perform a forensic investigation using Autopsy by creating a case, analyzing digital evidence, extracting artifacts, and generating a detailed forensic report.

---

## **Tools Used**
- Autopsy Forensic Tool
- Operating System: Windows/Linux
- Disk Image (E01, DD, IMG, RAW)

---

## **Procedure**

### **1. Create a New Case**
- Open Autopsy.
- Click **Create New Case**.
- Enter case name, number, examiner details.
- Choose case directory and click **Finish**.
<img width="842" height="530" alt="Image" src="https://github.com/user-attachments/assets/39199cfd-f2cf-4f90-ae2a-7f142e824b71" />

---

### **2. Add Data Source**
- Select **Add Data Source**.
- Choose **Disk Image** / **Local Drive**.
- Browse and load the evidence file.
- Configure ingest modules as required.

---

### **3. Monitor Ingest Progress**
- Autopsy will process the data source.
- Status and module progress can be viewed in the **Ingest Inbox**.

<img width="759" height="478" alt="Image" src="https://github.com/user-attachments/assets/bdb18612-4ac6-4e57-ba0e-f32bffa6eedc" />

---

### **4. View Artifacts**
Autopsy extracts multiple types of artifacts automatically:
- **Web History** (URLs, downloads, cookies)
- **Emails**
- **Installed Programs**
- **File System Structure**
- **User Activity**
- **Recent Documents**
- 
<img width="940" height="592" alt="Image" src="https://github.com/user-attachments/assets/585f46e3-52a7-40b8-8f21-4bfb95f1d6ad" />

---

### **5. Detailed Analysis**

#### ✅ Keyword Search
- Use keyword list or search bar for specific terms.

#### ✅ File System Browsing
- Explore directories, hidden files, deleted files.

#### ✅ Timeline Visualization
- View file activity in chronological order.

#### ✅ Hash Comparison
- Compare file hashes with known databases (NSRL, custom hash sets).

---


<img width="940" height="592" alt="Image" src="https://github.com/user-attachments/assets/911912ed-cb51-4a6f-8015-6ef50c0ffd16" />

- Go to **Generate Report**.
- Choose report format:
  - **HTML**
  - **CSV**
  - **Excel**
- Select the artifacts to include.
- Export and save the report.
- 

<img width="940" height="591" alt="Image" src="https://github.com/user-attachments/assets/e2dd85b5-22af-4624-a32f-f627bbf5811d" />

- 

---

### **7. Close Case & Archive**
- Close the case from the **Case Menu**.
- Archive the case for long-term storage.

---

## **Result**
- Successfully created a forensic case and analyzed digital evidence.
- Extracted multiple forensic artifacts.
- Generated a detailed investigation report using Autopsy.

---

## **Conclusion**
Autopsy provides a comprehensive digital forensic platform with powerful features for case management, artifact extraction, evidence analysis, and report generation. It is widely used for professional forensic investigations.

