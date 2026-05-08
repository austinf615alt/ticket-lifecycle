<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake to Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows Server 2025 Datacenter X64 Gen2</b> 

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution
  
<h2>Ticket Resolutions</h2>

<p>
<img width="2403" height="1216" alt="LAB2A-TicketTriage" src="https://github.com/user-attachments/assets/c3d2853f-e7a5-4878-9136-e10683d3bd28" />
</p>
<p>

- Intake: This ticket simulates a business critical outage affecting a bank’s online and mobile banking systems. The end user Karen reports that both services are down. It is originally marked as Normal priority with a default SLA under the "Other" Help Topic.
  
- Assignment and Communication: Tier 1 support would claim the ticket, confirming the issue scope with Karen by asking who and what is affected, verifying whether the outage is isolated or affecting multiple users. Confirming that the entire branch cannot access the online and mobile banking systems, the ticket is upgraded to an Emergency priority level with a high severity SLA classification and moved to the 'Business Critical" Help Topic.

- Working the Issue: Tier 1 support would initiate troubleshooting such as checking basic connectivity, and reviewing any recent service changes or known incidents. After follow-up, it is confirmed that the issue impacts the entire branch, indicating a system-wide outage.

- Resolution: Based on the ticket severity and business impact, the ticket is escalated to the SysAdmin team for further troubleshooting due to being out of tier 1 scope.

</p>
<br />

<p>
<img width="2403" height="1216" alt="LAB2A-TicketResolve2" src="https://github.com/user-attachments/assets/8af717cd-92e1-4b0a-8935-a20785f9e25e" />
</p>
<p>

- Intake: This ticket simulates an application failure affecting the Accounting department. End user Ken reports Adobe Reader does not launch and that 10 out of 12 of his coworkers cannot access it. It is originally marked as Normal priority with a default SLA under the "Personal Computers Issue" Help Topic.

- Assignment and Communication: Tier 1 would claim the ticket and communicate with the end user Ken to find out who and what is affected. Ken confirms that 10 of 12 users are unable to launch Adobe Reader, coinciding with an ongoing internal audit, which increases the business impact. Based on the scope and severity of the issue, the ticket is upgraded to a High Priority with a Medium SLA. The Help Topic is relevant.

- Working the Issue: Tier 1 troubleshooting includes remoting in to observe how the application behaves, confirming the issue persists after restarts and trying to launch it in safe mode. Further investigation shows that an Adobe Reader update deployed overnight has caused the application to stop launching.

- Resolution: A resolution is provided by the SysAdmin team, offering the end users either manual installation via the software catalog or waiting for a network-wide redeployment of a fixed package. The end user chooses to do a manual installation across the affected workstations, resolving the issue. Adobe Reader functionality is verified with the end user, and the ticket is closed.

</p>
<br />

<p>
<img width="2403" height="1216" alt="LAB2A-TicketResolve5" src="https://github.com/user-attachments/assets/d655e5b3-4bad-4135-bec6-d33dfe07fd5c" />
</p>
<p>

- Intake: This ticket simulates multiple scenarios within one ticket such as the only printer in the department not working, a computer being sluggish and Outlook application issues. End user Ken reports that the printer for the whole department is not printing despite the printer being powered on, online and loaded with paper. He also reports his computer is slow and his Outlook refuses to launch. It is originally marked as Normal priority with a default SLA under the "Personal Computer Issues" Help Topic.

- Assignment and Communication: Tier 1 support would claim the ticket and communicate with end user Ken to figure out the scope and impact. Ken reports that the entire department cannot print using the printer, which is the only one in the department. They also confirm that the slow PC and Outlook issues are isolated only to his system, with the PC being overall slow regardless of apps being open, and Outlook hanging when trying to be launched. Printer issue here takes priority due to its scope and business impact which determines that the ticket be upgraded to Emergency priority with a High SLA level and moved to the "Business Critical" Help Topic.

- Working the Issue: Tier 1 troubleshooting includes confirming the basics such as the printer having ink and paper, checking connectivity to see if it is online and powered on, and then reviewing the print queue/spooler. Investigation shows that the print queue is stuck, preventing print jobs from processing. Troubleshooting this issue is done by clearing the queue and restarting the print spooler service, which allows for the printer to work again. End user Ken confirms that they and others can print again and this incident is resolved.

  - Second issue of priority involves the slow PC issue. Basic trouleshooting is conducted such as checking what apps are open and looking in task manager to observe system resource usage. Task Manager observation shows that the PC has an unusually high uptime, causing performance issues. A resolution is provided by advising the end user to restart their computer to refresh system resources. End user Ken confirms the issue has been fixed and this incident is resolved.

  - Third issue of priority involves the Outlook issue. Basic troubleshooting is conducted such as verifying connectivity, restarting the app and system (already done), and testing Outlook in safe mode. It is observed that Outlook opens under safe mode, which indicates a likely issue with add-ins or user profile configuration. As a first step, optional add-ins are disabled, allowing Outlook to launch normally. Add-ins are then re-enabled individually to isolate the faulty component. After identifying and removing the problematic add-in, the end user verifies that Outlook functions normally. The incident is resolved and the ticket is fully closed.

</p>
<br />
