[Microsoft Applied Skills: Defend against cyberthreats with Microsoft Defender XDR](https://learn.microsoft.com/en-us/credentials/applied-skills/defend-against-cyberthreats-with-microsoft-defender-xdr/)

Date: 2026/07/30

---

Subject: General guidelines

From: cto@contoso.com
<br>
To: admin@WWLx559172.onmicrosoft.com

Thank you for agreeing to help our team defend against threats by using Microsoft Defender XDR.

We have some general guidelines that you must follow when you perform tasks in Azure. Please always use the following guidelines:

* When creating objects, use the default settings unless a different configuration is required to complete the task successfully.
* Only create, delete, or modify objects to achieve the stated requirements. Unnecessary changes to the environment can adversely affect your final score.
* If there are multiple approaches to achieving a goal, always choose the approach that requires the least amount of administrative effort.

Thanks,
<br>
Chief Technology Officer (CTO)

---

Subject: Existing environment

From: networkadmin@contoso.com
<br>
To: admin@WWLx559172.onmicrosoft.com

Here are your credentials for managing resources in Microsoft 365:

User name: admin@WWLx559172.onmicrosoft.com
<br>
Password: *********************

You can find these credentials by selecting the Instructions tab.

Your lab environment consists of two virtual machines named **Client1** and **Client2** that run Windows 11. Be sure to perform your tasks on the appropriate client as indicated in each email.
Before you begin, you must prepare Microsoft Defender XDR by performing the following steps:

* Sign in to **Client2** by using the provided credentials.
* Open Microsoft Edge, go to https://security.microsoft.com, and sign in.
* From the navigation pane, select **Investigation & response**, select **Incidents & alerts**, and then select **Incidents**. A message appears that states **Hang on! We're preparing new spaces for your data and connecting them**.

**Note: The message may remain for approximately five to 10 minutes.**

* After the message is no longer displayed, close Microsoft Edge. This will flush the web browser cache.
* Open Microsoft Edge, go to https://security.microsoft.com, and sign in.

Thanks,
<br>
Network Administrator

---

Subject: Onboard an endpoint to Microsoft Defender XDR

From: projman@contoso.com
<br>
To: admin@WWLx559172.onmicrosoft.com

Hello,

Now that we have provisioned Microsoft Defender XDR in our environment, we need you to create a new device group and onboard an endpoint client named **Client2**.

We will also run a sample attack script from **Client2** to simulate an attack.

This is your task:

First, you need to create a device group named **Group1** for Windows 10 and 11 devices. **Group1** must remediate all threats automatically.

Next, you need to onboard **Client2** to Microsoft Defender XDR. Store the onboarding script in the Downloads folder on **Client2**. Be sure that the onboarding process uses a connectivity type that recognizes simplified domains such as *.endpoint.security.microsoft.com.

**Note: It may take several minutes before Client2 displays in the Microsoft Defender portal.**

After **Client2** has been onboarded, simulate an attack by running the sample attack PowerShell script located at **C:\Files** on **Client2**. You can disregard the following message
displayed in the attack script: "Failed to resolve Domain Controllers in the domain."

Thanks,
<br>
Project Management Team

---

Subject: Create an Endpoint security policy

From: projman.@contoso.com
<br>
To: admin@WWLx559172.onmicrosoft.com

Hello,

We have reports company executives have downloaded and run a malicious JavaScript file on their devices. We need you to use Microsoft Defender to create a policy to address this
issue.

**Note: Complete this task from Client1.**

This is your task:

You need you to create an endpoint security policy named **EndpointPolicy1** and assign the policy to the **sg-Executive** security group. **EndpointPolicy1** must block Windows 1 1
devices from using JavaScript to download and run executable content.

Thanks,
<br>
Project Management Team

---

Subject: Manage a Microsoft Defender XDR incident

From: projman@contoso.com
<br>
To: admin@WWLx559172.onmicrosoft.com

Hello,

We have a Microsoft Defender DR incident named **Multi-stage incident involving Defense evasion & Discovery on one endpoint** that has been reported. We want you to
investigate the incident.

Note: Complete this task from **Client1**.

This is your task:

First, you need to review the device timeline of **Client2**. In the timeline, find the entry of the suspicious process injection that indicates the outbound connection to the malicious IP address and the target executable name that PowerShell performs process hollowing.

Next, create a custom indicator named **Indicator1** that will block execution when a user attempts to download a file from the malicious IP address. **Indicator1** must be assigned to
the **All devices in my organization** organizational scope and must generate a high severity alert for the **Execution** category.

Finally, create a detection rule named **SuspiciousPowershell** that runs every hour and is scoped to all devices. The rule must perform the following:

* Use the **DeviceProcessEvents** table and find powershell.exe events that will initiate the target executable found during the timeline review of **Client2**.
* Collect an investigation package.
* Mark the user that initiated the PowerShell process as compromised.

Thanks,
<br>
Project Management Team

---

Subject: Investigating and collecting forensic evidence from an endpoint

From: projman@contoso.com
<br>
To: admin@WWLx559172.onmicrosoft.com

Hello,

We need to use Microsoft Defender XDR to investigate and collect forensic evidence from **Client2**.

Note: Complete this task from **Client1**.

This is your task:

From **Client1**, perform the following tasks:
* Enable, and then initiate a live response session to **Client2** and view the current connections.
* Collect an investigation package from Client2, extract the **Forensics Collection Summary.csv** file from the package, and then save the file to C:\Files on **Client1**.
* Isolate **Client2**.

**Note: It may take a few minutes for the investigation package and isolation tasks to complete.**

Thanks,
<br>
Project Management Team

---

Subject: Status - Complete

From: cto@contoso.com
<br>
To: admin@WWLx559172.onmicrosoft.com

Thank you for helping our team defend against threats by using Microsoft Defender XDR.

We look forward to working with you again.

Regards,
<br>
Chief Technology Officer (CTO)