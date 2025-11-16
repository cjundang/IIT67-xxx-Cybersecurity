---
marp: true
theme: default
paginate: true
size: 16:9
title: "Cyber Threats in Healthcare Systems — Extended Lecture Edition"
---

# **Cyber Threats in Healthcare Systems**  
## **Week 2 — Threat Landscape & Ransomware Case Analysis**

---

# **Overview of Today’s Lecture**

### Part 1 — Healthcare Cyber Threat Landscape
- Why healthcare is heavily targeted  
- Key threat categories  
- Vulnerabilities in HIS/EMR/IoMT systems  
- Real-world threat statistics  


---

# **Overview of Today’s Lecture**

### Part 2 — Case Study: Ransomware
- Anatomy of a ransomware attack  
- Real hospital incidents  
- CIA impact analysis  
- Root cause exploration  
- Recovery & mitigation strategies  

### Part 3 — Summary & Self-Learning Tasks

---

# **Learning Objectives**

By the end of this session, students will be able to:

- Identify common cyber threats in healthcare  
- Explain why the healthcare sector is highly attractive to attackers  
- Analyze ransomware incidents using CIA Triad and root cause analysis  
- Recommend practical technical and administrative solutions  
- Develop deeper understanding through guided self-learning questions  

---

# **Section 1**  
# **Cyber Threats in Healthcare Systems**

---

# **Why Healthcare Is a Prime Target?**

### **1. High Value of Health Data**
- Medical identity = worth 20–50× more than credit card data  
- Can be used for blackmail, fraud, extortion

### **2. Critical Operations**
- Hospitals cannot tolerate downtime  
- Attackers exploit urgency → higher chance of ransom payment

### **3. Complex & Interconnected Systems**
- HIS–EMR–PACS–LIS–Billing  
- Many integration points → many attack surfaces

---

# **Why Healthcare Is a Prime Target?**


### **4. Legacy Devices & Weak Security**
- Outdated OS (Windows 7, XP) on medical equipment  
- IoMT devices rarely patched

### **5. High Human Error Rate**
- Busy clinical environment → more likely to fall for phishing

---

# **Threat Landscape Visual (Self-Learning Aid)**

- **82%** of healthcare breaches involve human error (Verizon DBIR)  
- **70%** of hospitals experienced ransomware in the past 3 years  
- **45%** of IoMT devices have known vulnerabilities  
- Average cost of healthcare breach: **USD 11 million**

> **Reflection:**  
> Why is healthcare consistently the *most expensive* industry for data breaches?

---

# **Common Threat Categories**

### 🔹 **Malware**
- Infects hospital systems  
- May steal data or destroy files  

### 🔹 **Ransomware**
- Encrypts EMR/PACS systems  
- Demands payment for decryption  

### 🔹 **Phishing / Social Engineering**
- Most successful initial attack vector  
- Often impersonates clinicians or admin staff  

---

# **Common Threat Categories**


### 🔹 **Insider Threats**
- Malicious: stealing data  
- Accidental: mis-sending patient data  

### 🔹 **IoMT Attacks**
- Unsafe wireless infusion pumps  
- Vulnerable PACS servers  
- Weak/no authentication

---

# **Examples of Threat Actions**

- EMR data theft  
- Unauthorized modification of patient history  
- Hijacked radiology imaging servers  
- Shutdown of critical-care systems  
- Alteration of lab test results  
- Access to medication dispensing systems  

---

# **Deep Dive: Malware Types in Healthcare**

### **1. Keyloggers**
- Capture clinician credentials  
- Used to access EMR systems

### **2. Remote Access Trojans (RATs)**
- Attackers take full control of hospital servers

### **3. Worms**
- Spread automatically across internal networks  
- Example: WannaCry shut down NHS (UK) hospitals

---

# **Phishing in Healthcare (Detailed View)**

### **Why phishing works well:**
- High email traffic in hospitals  
- Lack of cybersecurity training  
- Staff under time pressure  
- Many external communications (labs, insurance, referrals)

### **Common phishing themes:**
- Fake lab order requests  
- Fake insurance claims  
- Fake IT support emails  
- Fake system updates  

---

# **Insider Threat Examples**

### **Accidental:**
- Sending lab results to wrong patient  
- Losing unencrypted USB drive  
- Misconfigured access permissions

### **Malicious:**
- Employee sells patient data  
- Unauthorized system access  
- Data deletion after termination

---

# **IoMT Vulnerabilities**

- Weak encryption on wireless vital sign monitors  
- Default manufacturer passwords  
- Unsupported/obsolete firmware  
- PACS often runs on outdated Windows servers  
- Unsegmented network → attackers jump from IoMT to EMR

---

# **Section 2**  
# **Ransomware in Healthcare**

---

# **What is Ransomware?**

### **Definition**
Malware that encrypts hospital data and disables systems until ransom is paid.

### **Key Characteristics**
- Fast propagation  
- Targets critical systems (EMR, LIS, PACS)  
- Double-extortion:  
  - Encrypt data  
  - Steal data → leak if unpaid  

---

# **What is Ransomware?**


### **Why Healthcare Is Highly Vulnerable**
- High urgency = high likelihood of ransom payment  
- Legacy systems  
- Limited downtime tolerance  

---

# **Ransomware Attack Flow**

### **1. Reconnaissance**
- Identify weak hospital endpoints  
- Scan for exposed RDP ports  

### **2. Initial Compromise**
- Phishing email → credential theft  
- Unpatched VPN appliance  

### **3. Lateral Movement**
- Move from one system to another  
- Search for domain controller  

---

# **Ransomware Attack Flow**


### **4. Privilege Escalation**
- Admin account compromise  

### **5. Data Exfiltration**
- Steal EMR or patient scans  

### **6. Encryption**
- Lock critical systems  
- Deploy encryption across servers  

---

# **Ransomware Attack Flow**


### **7. Ransom Demand**
- Typically via TOR  
- Payment in cryptocurrency  

---

# **Real Example: WannaCry (NHS, UK)**

- Impacted **80+ hospitals**  
- Caused cancelled surgeries and treatment delays  
- Targeted outdated Windows XP machines  
- NHS estimated impact: **£92 million**

---

# **Real Example: Düsseldorf University Hospital (Germany)**

- Ransomware caused ER shutdown  
- Ambulances rerouted → critical delay  
- One patient died en route  
- First recorded ransomware-linked fatality

---

# **Case Study Scenario for Analysis**

### **Hospital X Incident**

- A nurse received an email labeled **“Urgent: Lab Results Delay Notice”**  
- Link → malicious login page  
- Credentials stolen  
- Attackers accessed EMR server  
- Ransomware deployed at 2 AM  
- Hospital forced to switch to paper documentation  
- Attackers demanded **250,000 USD**

---

# **CIA Triad Impact Assessment**

### **Confidentiality**
- Patient records leaked  
- Billing data exposed  
- Lab results stolen  

### **Integrity**
- Records may be altered  
- Misdiagnoses possible  
- Medication orders compromised  

---

# **CIA Triad Impact Assessment**

### **Availability**
- EMR offline  
- PACS imaging unavailable  
- Surgeries and appointments cancelled  

---

# **Root Cause Analysis**

### **Technical**
- Outdated OS  
- Missing patches  
- Weak antivirus  
- Flat network architecture  

### **Procedural**
- No multi-factor authentication  
- Weak backup strategy  
- Lack of network segmentation  

---

# **Root Cause Analysis**

### **Human**
- Staff untrained in phishing  
- Poor password hygiene  
- No incident response practice  

---

# **Recovery & Mitigation Strategies**

### **Immediate Response**
- Isolate infected systems  
- Switch to manual operations  
- Notify authorities  
- Begin forensic investigation  


---

# **Recovery & Mitigation Strategies**

### **Long-Term Improvements**
- Implement MFA  
- Offline/immutable backups  
- Patch management program  
- Security awareness training  
- Zero trust architecture  
- Network segmentation (IoMT isolation)  

---

# **Section 3**  
# **Group Activity: Ransomware Analysis**

---

# **Activity Tasks**

### **Each group (4–5 students) will:**
1. Review the ransomware scenario  
2. Identify affected systems  
3. Map impacts to CIA Triad  
4. Identify root causes  
5. Propose mitigation strategies  

### **Deliverables**
- 3–5 minute group presentation  
- Short written analysis (optional homework)

---

# **Guided Self-Learning Questions**

1. Which system in a hospital is most vulnerable to ransomware? Why?  
2. How does ransomware spread between departments?  
3. What human behaviors increase ransomware risks?  
4. What would be your top priority during recovery?  
5. Should hospitals ever pay ransom? Discuss the pros/cons.

---

# **Additional Reading for Self-Learning**

- HC3 (U.S. HHS) Hospital Ransomware Reports  
- WHO Cybersecurity in Healthcare Guidelines  
- NIST SP 800-53 Security Controls  
- ENISA Threat Landscape Reports  
- IEEE Healthcare Security Research Articles  

---

# **Section 4**  
# **Summary**

---

# **Key Takeaways**

- Healthcare is one of the most targeted sectors globally  
- Cyber threats are diverse: malware, ransomware, phishing, insider threats  
- IoMT greatly expands the attack surface  
- Ransomware causes major operational and patient safety risks  
- Prevention requires technical, administrative, and human-based defenses  
- Preparedness through training and incident rehearsal is essential  

---

# **Thank You**
## **Week 2 Lecture Completed**
Questions and further discussion are welcome.
