<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake to Resolution</h1>
This project outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket

<h2>Operating Systems Used</h2>

- Windows Server 2025 Datacenter X64 Gen2

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Ticket Resolutions</h2>

## Ticket 1: Intake

---

<p>
<img width="1624" height="979" alt="Ticket Create" src="https://github.com/user-attachments/assets/49716374-0445-473f-bb0e-5492ee0700bb" />
</p>
<p>

- Simulated end-user ticket submission by logging into the osTicket end-user portal as **Karen** and submitting a new ticket reporting that the **entire mobile/online banking system was down**, affecting all customers and internal users.

</p>
<br />

<p>
<img width="1624" height="979" alt="John Login" src="https://github.com/user-attachments/assets/2f607e8a-4f1a-4448-917a-0417070da93e" />
</p>
<p>

- Authenticated into the Agent Panel as Help Desk Agent **John** to begin the triage process and review incoming tickets from the queue.

</p>
<br />

<p>
<img width="1624" height="979" alt="John Opens Ticket" src="https://github.com/user-attachments/assets/3df026ca-27ef-4336-815c-afb0301c75dc" />
</p>
<p>

- Opened the incoming ticket as **John** to assess its default properties — noting that **Priority**, **Department**, **SLA**, and **Assigned To** were all unset, reflecting the raw state of a ticket prior to triage.

</p>
<br />

## Ticket 1: Assignment and Communication

---

<p>
<img width="1624" height="979" alt="John Triage 1" src="https://github.com/user-attachments/assets/1fadce09-6aaa-442c-852d-e9d76cded92e" />
</p>
<p>

- Initiated simulated contact with the end user to gather additional details. Based on the reported impact — a complete outage of the mobile and online banking platform — escalated the ticket **Priority** to **Emergency**, reflecting the critical business impact and urgency of the issue.

</p>
<br />

<p>
<img width="1624" height="979" alt="SLA Update" src="https://github.com/user-attachments/assets/a047dd90-b557-40fe-b9af-4ec46dd98464" />
</p>
<p>

- Updated the **SLA Plan** to **Sev-A** (1-hour grace period, 24/7 schedule), appropriate given that a full banking system outage constitutes a business-critical incident requiring immediate around-the-clock resolution.

</p>
<br />

<p>
<img width="1624" height="979" alt="Update Help Topic" src="https://github.com/user-attachments/assets/c13c0988-e2c0-4f45-a3ab-56b7a7aab9fc" />
</p>
<p>

- Updated the **Help Topic** to **Business Critical Outage** to accurately reflect the nature of the issue — a system-wide banking platform failure affecting branch operations — ensuring proper categorization for reporting and routing purposes.

</p>
<br />

<p>
<img width="1624" height="979" alt="Reassigned Jane" src="https://github.com/user-attachments/assets/a228d5e8-9616-40c2-a42b-729f1aa77928" />
</p>
<p>

- Reassigned the ticket to agent **Jane** (SysAdmins department), as the severity and scope of the outage exceeded Tier 1 support capabilities. The ticket was escalated to a SysAdmin with the permissions and expertise required to investigate and remediate a platform-level failure.

</p>
<br />

<p>
<img width="1624" height="979" alt="Transfer Sysadmins" src="https://github.com/user-attachments/assets/5df8fd7b-dd41-4c58-9772-d391e563e64e" />
</p>
<p>

- Transferred the ticket's **Department** to **SysAdmins**, aligning the ticket's ownership with the team responsible for infrastructure-level resolution and ensuring proper departmental routing within osTicket.

</p>
<br />

<p>
<img width="1624" height="979" alt="John Lost Access" src="https://github.com/user-attachments/assets/b88b8798-ce91-4809-8896-2496e5a2ba7e" />
</p>
<p>

- Verified osTicket's **department-based access control** by attempting to view the transferred ticket as **John**. As expected, John no longer had visibility into the ticket after it was moved to the SysAdmins department — confirming that ticket access is properly scoped to department membership.

</p>
<br />

## Ticket 1: Working the Issue

---

<p>
<img width="1624" height="979" alt="Jane Login" src="https://github.com/user-attachments/assets/c38795f3-15c1-4ce6-863a-0e89a8a47b6b" />
</p>
<p>

- Authenticated into the Agent Panel as **Jane** (Super Admin role) to take ownership of the escalated ticket and begin active investigation of the banking system outage.

</p>
<br />

<p>
<img width="1624" height="979" alt="Jane Opens Ticket" src="https://github.com/user-attachments/assets/81dd60d8-acdc-4580-a8c8-5810c01d1a23" />
</p>
<p>

- Opened the ticket as **Jane** to review the full ticket history, triage notes left by John, and all updated properties — including the Sev-A SLA, Emergency priority, and Business Critical Outage classification — before proceeding with investigation.

</p>
<br />

<p>
<img width="1624" height="979" alt="Jane Reply" src="https://github.com/user-attachments/assets/c9085a16-c30d-4ab3-acac-3c32ef481657" />
</p>
<p>

- Posted an internal update and reply to the end user outlining the suspected root cause of the outage and the remediation steps being taken, maintaining transparent communication throughout the resolution process in accordance with SLA expectations.

</p>
<br />

## Ticket 1: Resolution

---

<p>
<img width="1624" height="979" alt="Jane Fix" src="https://github.com/user-attachments/assets/c38872ca-3a69-4da8-a810-b241121189f3" />
</p>
<p>

- Confirmed that the applied fix successfully restored the mobile and online banking system. Communicated resolution status to the end user and documented the fix within the ticket thread for documentation purposes.

</p>
<br />

<p>
<img width="1624" height="979" alt="Ticket Close" src="https://github.com/user-attachments/assets/242d834d-4a25-4e10-b494-51ebfe83e37c" />
</p>
<p>

- Verified full service restoration and closed the ticket as **Closed**. The complete lifecycle — from end-user submission through Tier 1 triage, SysAdmin escalation, and resolution — was documented within the ticket thread.

</p>
<br />

---

## Ticket 2: Intake

---

<p>
<img width="1624" height="981" alt="Ticket 2 Creation" src="https://github.com/user-attachments/assets/334462cc-bbe1-4fdf-a58b-5c33e068d255" />
</p>
<p>

- Simulated end-user ticket submission by logging into the osTicket portal as **Ken** and submitting a ticket reporting that **Adobe Reader was broken for the Accounting department**.

</p>
<br />

<p>
<img width="1624" height="979" alt="John Login x2" src="https://github.com/user-attachments/assets/deb83adb-c857-456e-a5b9-ac0761805b9b" />
</p>
<p>

- Signed into the Agent Panel as Help Desk Agent **John** to begin reviewing the newly submitted ticket from the queue.

</p>
<br />

<p>
<img width="1624" height="979" alt="John Opening Ticket" src="https://github.com/user-attachments/assets/35b7a632-9f4c-40f7-89ce-336abdc61e44" />
</p>
<p>

- Opened the ticket as **John** to assess its initial properties. Reviewed the reported issue — Adobe Reader non-functional for some in the Accounting department — and noted that **Priority**, **SLA**, **Department**, and **Assigned To** were all pending triage assignment.

</p>
<br />

## Ticket 2: Assignment and Communication

---

<p>
<img width="1624" height="979" alt="Scope Investigation" src="https://github.com/user-attachments/assets/b537588b-1ff1-4c0c-a076-bd1f2a143a7f" />
</p>
<p>

- Conducted scope investigation by contacting end user **Ken** directly to determine the impact scope. Confirmed that **10 out of 12 Accounting staff** were affected and that the outage was particularly time-sensitive given an **active internal audit** in progress, elevating the business urgency of the ticket.

</p>
<br />

<p>
<img width="1624" height="979" alt="Priority Level Change" src="https://github.com/user-attachments/assets/7b7e83ac-d367-438d-aa1e-d96a9af932ad" />
</p>
<p>

- Escalated the ticket **Priority** to **High** based on the number of affected users and the time-sensitive nature of the ongoing audit, documenting the rationale within the ticket thread to maintain a clear triage record.

</p>
<br />

<p>
<img width="1624" height="979" alt="SLA Change" src="https://github.com/user-attachments/assets/e356e034-cdf3-4259-9f1d-024359568f01" />
</p>
<p>

- Updated the **SLA Plan** to **Sev-B** (4-hour grace period, 24/7 schedule) and assigned the ticket to the **Support** department. The Sev-B classification was appropriate given the high user impact and audit deadline sensitivity, while stopping short of Sev-A since core infrastructure remained operational.

</p>
<br />

## Ticket 2: Working the Issue

---

<p>
<img width="1624" height="979" alt="Root Cause Analysis" src="https://github.com/user-attachments/assets/7e37cba3-3f45-4f6a-87be-b36c1738b86c" />
</p>
<p>

- Escalated internally by coordinating with **Austin from the Admin group** to identify the root cause. Determined that a **faulty Adobe Reader package had been pushed out the previous night**, making the application non-functional across the affected workstations. Identified two fixes: waiting one hour for a corrected package to be deployed automatically, or having end users manually install the updated package immediately. Communicated both options to the end user.

</p>
<br />

<p>
<img width="1624" height="979" alt="Fix Verified" src="https://github.com/user-attachments/assets/fabe4493-93e4-4714-ab42-4d30f31792c6" />
</p>
<p>

- Received confirmation from end user **Ken** that the manual installation of the fixed Adobe Reader package was successful across all affected machines. All 10 impacted Accounting staff members were restored to full functionality in time to support the ongoing audit.

</p>
<br />

## Ticket 2: Resolution

---

<p>
<img width="1624" height="979" alt="Ticket 2 Close" src="https://github.com/user-attachments/assets/9f255d67-8285-4b3b-b123-357fc7cce242" />
</p>
<p>

- Documented the confirmed fix — a faulty package deployment corrected via manual reinstallation — and officially closed the ticket. The full ticket lifecycle, including scope investigation, SLA assignment, root cause analysis, and end user communication, was captured within the ticket thread for future reference.

</p>
<br />

---

## Skills Developed

### Help Desk Triage & Ticket Management
Practiced the full ticket lifecycle within a real ticketing platform — from initial intake and ticket observation through escalation, active resolution, and closure. Developed the ability to evaluate unset ticket properties and apply accurate classifications based on reported symptoms and business impact.

### SLA Prioritization & Severity Assessment
Applied SLA frameworks in context, distinguishing between Sev-A (1-hour, 24/7) and Sev-B (4-hour, 24/7) classifications based on scope of impact, number of affected users, and business-critical dependencies such as active audits and customer-facing service outages.

### Escalation & Cross-Tier Coordination
Demonstrated sound escalation judgment by identifying when a ticket exceeded Tier 1 scope and routing it to the appropriate SysAdmin agent and department. Coordinated across teams (Support, SysAdmins, Admin group) to conduct root cause analysis and deliver a resolution within SLA.

### Role-Based Access Control (RBAC) Validation
Observed and documented osTicket's department-based access control behavior — verifying that agents lose ticket visibility upon department reassignment — confirming a practical understanding of how RBAC governs ticket security in enterprise help desk environments.

### Root Cause Analysis & Documentation
Investigated a software deployment failure (faulty Adobe Reader package) by coordinating with internal stakeholders, identifying the source of the issue, and presenting multiple remediation paths to the end user. Documented findings, actions taken, and resolution outcomes within the ticket thread.

### End-User Communication & Expectation Management
Maintained clear, professional communication with end users throughout each ticket lifecycle — setting expectations, providing status updates, presenting remediation options, and confirming resolution before closure, reflecting real-world ITSM best practices.

### IT Service Management (ITSM) Fundamentals
Gained hands-on experience with core ITSM concepts including incident classification, priority management, ticket ownership, departmental routing, and structured resolution workflows — all executed within an industry-standard help desk platform.
