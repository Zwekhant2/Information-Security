# Assignment: Kill Chain

## x) Read and summarize

### Hutchins et al. 2011: Intelligence-Driven Computer Network Defense

**Summary:**
- The **Cyber Kill Chain** is a framework to stop attackers by understanding their steps.
- The seven steps are:  
  1. **Reconnaissance**: Attackers gather information about the target.  
  2. **Weaponization**: Attackers create malicious tools like malware.  
  3. **Delivery**: They send the malicious tools (e.g., phishing email).  
  4. **Exploitation**: They use vulnerabilities to launch the attack.  
  5. **Installation**: The attacker sets up a foothold in the system.  
  6. **Command and Control (C2)**: They control the system remotely.  
  7. **Actions on Objectives**: The attacker completes their goal (e.g., stealing data).  
- The goal is to stop the attack at any stage using intelligence and defensive strategies.

**Question/Insight:** How can we automate tools to stop attackers at different steps of the Kill Chain?

### MITRE ATT&CK Matrix for Enterprise

**Summary:**
- MITRE ATT&CK is a framework that explains how attackers act (Tactics, Techniques, and Procedures).  
- **Tactic**: The attack’s goal (e.g., gaining access).  
- **Technique**: How the goal is achieved (e.g., stealing passwords).  
- **Subtechnique**: A detailed method (e.g., stealing from memory).  
- **Procedure**: Specific tools or methods attackers use (e.g., using PowerShell scripts).  
- Helps defenders predict and stop real-world attacks.

**Question/Insight:** Can we use AI to predict what attackers might do next based on this framework?

---

## a) Tactics, Tools, and Procedures

### Tactic
- **Definition**: The goal of an attacker’s action.  
- **Example**: **Persistence** – The attacker keeps access by creating fake user accounts.

### Technique
- **Definition**: The method used to achieve a tactic.  
- **Example**: **Scheduled Task/Job (T1053)** – The attacker schedules malicious programs to run later.

### Subtechnique
- **Definition**: A specific way to perform a technique.  
- **Example**: **Scheduled Task (T1053.005)** – Using Windows Task Scheduler to run malware.

### Procedure
- **Definition**: The exact tool or script used for an attack.  
- **Example**: An attacker uses PowerShell to create a malicious scheduled task.

---

## c) Voluntary Bonus: Attack Story

### Example Attack Story

1. **Initial Access**:  
   - **Technique:** Phishing (T1566).  
   - **Procedure:** An attacker sends an email with a malicious link.

2. **Execution**:  
   - **Technique:** User Execution (T1204).  
   - **Procedure:** The victim clicks the link, and malware is installed.

3. **Persistence**:  
   - **Technique:** Create Account (T1136).  
   - **Procedure:** The malware adds a new administrator account.

4. **Defense Evasion**:  
   - **Technique:** Obfuscated Files (T1027).  
   - **Procedure:** The malware hides its code to avoid being detected.

**Defensive Actions:** Use phishing filters, tools to spot unusual behavior, and security software to detect malware.

---

### References
1. Hutchins, E. M., Cloppert, M. J., & Amin, R. M. (2011). Intelligence-Driven Computer Network Defense.
2. MITRE ATT&CK Framework: [https://attack.mitre.org](https://attack.mitre.org)
