# THM-Writeup-SOAR
Writeup for TryHackMe SOAR Lab - Automated threat detection and response using SOAR to streamline phishing analysis, CVE patching, and incident management.

By Ramyar Daneshgar


### **Task 1: Understanding SOC Evolution and Challenges**

#### **Step Taken: Studying SOC Generations**
I reviewed the **evolution of Security Operations Centers (SOCs)** to understand their development from basic monitoring systems to modern-day threat intelligence hubs. 

- **First-Generation SOCs**: Focused on basic log collection and antivirus monitoring.
- **Second-Generation SOCs**: Introduced **SIEMs (Security Information and Event Management)**, enabling event correlation and initial threat management.
- **Fourth-Generation SOCs**: Integrated **big data analytics**, real-time threat intelligence, and advanced detection tools.

#### **Key Cybersecurity Insight:**
I identified how SOCs have transitioned into proactive threat detection platforms by adopting automated tools to combat challenges like **alert fatigue** and **disparate tool management**.

---

### **Task 2: Learning SOAR Basics**

#### **Step Taken: Exploring SOAR Concepts**
I delved into the key components of **Security Orchestration, Automation, and Response (SOAR)**:

1. **Orchestration**: Integration of disparate security tools into cohesive workflows to streamline operations.
2. **Automation**: Using playbooks to handle repetitive tasks like IOC analysis or malware removal.
3. **Response**: Automating triage and remediation to reduce **MTTD (Mean Time to Detect)** and **MTTR (Mean Time to Respond)**.

#### **Practical Difference Between SOAR and SIEM**:
I noted that SOAR enhances SIEM capabilities by automating **incident response workflows**, minimizing human intervention, and enabling end-to-end threat management.

---

### **Task 3: SOAR Workflow Scenarios**

#### **Phishing Workflow**
I analyzed the **phishing workflow** scenario provided:

1. **Sandbox Analysis**:
   - Isolated suspicious emails in a sandbox to mitigate potential threats.
   - Parsed **IOCs (Indicators of Compromise)** such as URLs, attachments, and file hashes.

2. **Threat Intel Integration**:
   - Used tools like VirusTotal to enrich IOCs with additional context.
   - Verified the legitimacy of extracted URLs and attachments through hash analysis.

3. **Automated Remediation**:
   - Deleted malicious emails.
   - Updated the case management system and communicated results with stakeholders.

#### **CVE Patching Workflow**
I studied the **CVE patching workflow**, which emphasized automation in vulnerability management:

1. **CVE Monitoring**:
   - Pulled real-time CVE data from advisory feeds.
   - Queried the internal patch management system for unpatched vulnerabilities.

2. **Patch Deployment**:
   - Tested patches in virtual environments to minimize production risks.
   - Performed **post-deployment vulnerability scans** to verify successful remediation.

#### **Key Takeaway:**
These workflows demonstrated how SOAR automates repetitive tasks while enabling **incident triage**, **root cause analysis**, and **remediation tracking**.

---

### **Task 4: Practical Workflow Implementation**

#### **Scenario Overview**:
In this practical exercise, I configured a SOAR platform to automate a **threat intelligence integration workflow**. Below is the detailed breakdown of steps:

1. **Workflow Initialization**:
   - Set up triggers to detect incoming security events.
   - Configured integration points for threat feeds and IOC parsing.

2. **IOC Enrichment**:
   - Integrated tools like VirusTotal to automatically analyze file hashes and URLs.
   - Enriched detection data with **TTPs (Tactics, Techniques, and Procedures)** to understand adversary behavior.

3. **Automated Case Management**:
   - Configured SOAR to open tickets automatically in TheHive for tracking incidents.
   - Ensured all enriched data and analysis were logged systematically.

4. **Validation and Testing**:
   - Tested the workflow to ensure seamless automation.
   - Resolved any errors to achieve a fully functional threat intelligence flow.

#### **Flag Retrieval**:
Upon successful execution, I retrieved the flag: **THM{AUT0M@T1N6_S3CUR1T¥}**.

---

### **Key Takeaways from the Room**

1. **Enhanced Incident Response**:
   - SOAR drastically reduces manual intervention by automating workflows like phishing analysis and CVE patching.
   - This leads to faster threat containment and minimizes damage.

2. **Integration-First Approach**:
   - SOAR’s ability to unify disparate tools, such as SIEMs and threat intel feeds, ensures better visibility and context for SOC analysts.

3. **Data Security**:
   - Enrichment of IOCs using real-time intelligence adds layers of accuracy and reduces false positives.

4. **Operational Metrics**:
   - SOAR workflows reduce **MTTD** and **MTTR**, critical KPIs for measuring SOC efficiency.
