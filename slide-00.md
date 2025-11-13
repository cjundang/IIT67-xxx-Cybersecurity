---
marp: true
title: ITD62-332 Cybersecurity — Course Syllabus (มคอ.3)
paginate: true
theme: default
---

# **ITD62-332 ความมั่นคงไซเบอร์**  
## *(Cybersecurity)*  
ภาคการศึกษา 2/2568 — 3(2–2–5)

ผู้สอน: ผู้ช่วยศาสตราจารย์ ดร.ชนันท์กรณ์ จันแดง  
หลักสูตรนวัตกรรมสารสนเทศทางการแพทย์ / IT และนวัตกรรมดิจิทัล

---

# **1. รหัสและชื่อรายวิชา**

**ภาษาไทย:** ITD62-332 ความมั่นคงไซเบอร์  
**ภาษาอังกฤษ:** Cybersecurity  

**จำนวนหน่วยกิต:** 3(2–2–5)  
- บรรยาย 2 ชม.  
- ปฏิบัติการ 2 ชม.  
- ศึกษาค้นคว้า 5 ชม.

---

# **2. รายวิชาในหลักสูตร**

อยู่ในหมวด  
**โครงสร้างพื้นฐานของระบบ (System Infrastructure)**  
สำหรับ 2 หลักสูตร  
- นวัตกรรมสารสนเทศทางการแพทย์  
- เทคโนโลยีสารสนเทศและนวัตกรรมดิจิทัล

---

# **3. ผู้สอนและภาคที่เปิดสอน**

**ผู้ประสานงาน/ผู้สอน:**  
ผู้ช่วยศาสตราจารย์ ดร.ชนันท์กรณ์ จันแดง

**ภาคการศึกษา:** 2  
**รายวิชาที่ต้องเรียนมาก่อน:** ITD62-231 เทคโนโลยีอินเทอร์เน็ต  
**เรียนพร้อมกัน:** ไม่มี

---

# **4. คำอธิบายรายวิชา**

ศึกษาหลักการความมั่นคงไซเบอร์ ภัยคุกคาม ช่องโหว่ การวิเคราะห์ทราฟฟิกเครือข่าย การใช้เครื่องมือด้านความมั่นคงไซเบอร์   การจัดการบันทึกเหตุการณ์ การตรวจจับการบุกรุก   รวมถึงการใช้เทคนิคปัญญาประดิษฐ์เพื่อตรวจจับความผิดปกติเชิงลึก   มุ่งพัฒนาทักษะการคิดวิเคราะห์และจริยธรรมวิชาชีพด้านไซเบอร์

---

# **5. ผลการเรียนรู้ของรายวิชา (CLOs)**

### **ด้านความรู้**  
- **CLO1:** อธิบายหลักการพื้นฐานความมั่นคงไซเบอร์และภัยคุกคาม  
- **CLO2:** อธิบายโปรโตคอลเครือข่ายและมาตรฐานความมั่นคงไซเบอร์  

### **ด้านทักษะ**
- **CLO3:** วิเคราะห์ทราฟฟิกเครือข่ายและระบุพฤติกรรมผิดปกติ  
- **CLO4:** ใช้ Wireshark, Suricata, Firewall, Log Tools  
- **CLO5:** พัฒนา ML Model เพื่อตรวจจับมัลแวร์/ความผิดปกติ  

### **ด้านคุณธรรม**
- **CLO6:** ปฏิบัติงานภายใต้กฎหมายและจริยธรรมไซเบอร์

---

# **6. แผนการสอน 12 สัปดาห์ (Integrated Plan)**

| **Week** | **Topic**                                                                                  | **Lecture**                                                            | **Workshop / Lab**                            | **Assessment**    |
| -------- | ----------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- | --------------------------------------------- | ----------------- |
| **1**    | Intro. to Cybersecurity          | CIA/DAD Principles, Threat–Vulnerability, Security as Asset Protection | Analysis of real cyberattack scenarios        | Quiz + Report     |
| **2**    | Network and Protocol Fundamentals | IP, Subnetting, OSI/TCP-IP, Protocol Weaknesses                        | Packet Flow Analysis                          | Worksheet         |
| **3**    | Network Traffic Analysis with Wireshark and Advanced Packet Filtering Techniques                      | Packet Dissection, Filters, PyShark                                    | Wireshark Lab + PyShark Scripting             | Lab Report        |
| **4**    | Cyber Threats, Attack Techniques, and Network Security Troubleshooting                                | Malware, DoS, MITM, ARP Spoofing                                       | ARP Spoofing Simulation + Detection           | Quiz + Lab        |
| **5**    | Firewall Concepts and Network Access Control (ACL, NAT, Stateful Inspection)                          | ACL, Stateful Inspection, NAT/PAT                                      | ACL & Firewall Configuration (Packet Tracer)  | Lab Assignment    |

---
| **Week** | **Topic**                                                                                  | **Lecture**                                                            | **Workshop / Lab**                            | **Assessment**    |
| -------- | ----------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- | --------------------------------------------- | ----------------- |
| **6**    | Enterprise LAN Security and Switch-Level Defense Mechanisms                                           | VLAN, Port Security, DHCP Snooping, Dynamic ARP Inspection (DAI)       | LAN Attack Surface Simulation                 | Lab               |
| **7**    | Malware Detection Using Machine Learning: PE File Features and ML Algorithms                          | Malware Taxonomy, PE Feature Engineering, ML Algorithms                | Model Training + Performance Evaluation       | ML Lab            |

---
| **Week** | **Topic**                                                                                  | **Lecture**                                                            | **Workshop / Lab**                            | **Assessment**    |
| -------- | ----------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- | --------------------------------------------- | ----------------- |
| **8**    | Network Traffic Anomaly Detection with Machine Learning and NetFlow                                   | NetFlow, Feature Engineering, Isolation Forest                         | Flow Dataset Construction + Anomaly Detection | Coding Assignment |
| **9**    | Log and Audit Log Management with Logging Standards and the ELK Stack                                 | Log Standards, ELK Stack Architecture, Operational Challenges          | FastAPI Log Pipeline + React-Based Dashboard  | Log Lab           |

---
| **Week** | **Topic**                                                                                  | **Lecture**                                                            | **Workshop / Lab**                            | **Assessment**    |
| -------- | ----------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- | --------------------------------------------- | ----------------- |
| **10**   | Intrusion Detection and Prevention Systems (IDS/IPS) Using Snort and Suricata                         | IDS Rule Syntax, EVE JSON, Rule Tuning                                 | Attack Simulation + Alert Analysis            | IDS Lab           |
| **11**   | Security Automation and Intelligent IDS: AI/ML-enhanced Detection and Automated Security Pipelines    | ML-driven IDS, WebSocket Security Pipeline                             | Intelligent IDS Prototype Development         | Project Lab       |
---
| **Week** | **Topic**                                                                                  | **Lecture**                                                            | **Workshop / Lab**                            | **Assessment**    |
| -------- | ----------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- | --------------------------------------------- | ----------------- |
| **12**   | Integration of Cybersecurity Knowledge and Skills from a Security Operations Center (SOC) Perspective | SOC Concepts, Course Summary                                           | Practical Exam + Final Presentation           | Practical Exam    |

---

# **7. วิธีประเมินผล**

| รายการประเมิน | สัดส่วน | รายละเอียด |
|---|---|---|
|แบบทดสอบ/แบบฝึกหัด|20%|ทฤษฎีและวิเคราะห์ภัยคุกคาม|
|งานปฏิบัติการ (Labs)|30%|Wireshark, IDS, ML Detection|
|งานวิเคราะห์/รายงาน|20%|Log Analysis, Attack Investigation|
|สอบกลางภาค|10%|ทฤษฎีความมั่นคงไซเบอร์|
|สอบปลายภาค|20%|Practical + Written|

---

# **8. มาตราการจัดการเรียนรู้**

- บรรยายเชิงวิเคราะห์  
- ทดลองปฏิบัติการ  
- วิเคราะห์เหตุการณ์จริง  
- Workshop และ Coding Lab  
- Case-based Learning  
- Ethical Discussion

---

# **9. Learning Resources**

- เอกสารประกอบการสอน  
- Wireshark, Suricata, FastAPI, ReactJS  
- Packet Tracer, Python (pandas, scikit-learn)  
- ISO 27001, NIST 800-series  
- CERT Incident Reports  

---