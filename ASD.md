## **ASD Essential 8 (now ACSC)**

-   **Please start with this - ACSC Essential 8 – Health Report in Microsoft Sentinel**
<https://techcommunity.microsoft.com/blog/microsoftsentinelblog/acsc-essential-8-%e2%80%93-health-report-in-microsoft-sentinel/3755702>
![](https://techcommunity.microsoft.com/t5/s/gxcuf89792/images/bS0zNzU1NzAyLTQ0NjUxNGkzM0RCODE5QjU4RjA2MEJB)

-   [Microsoft's guidance on Essential 8 implementation](https://aka.ms/e8guides)
-   [Collection of Australian M365 content on Essential 8](https://m365maps.com/australia.htm)
-   [Microsoft Cybersecurity Reference Architecture](https://aka.ms/MCRA)
-   [Australian IRAP](https://learn.microsoft.com/en-us/azure/compliance/offerings/offering-australia-irap)
-   Licencing required to implment Essential 8 with Microsoft tooling
![](./images/Essential-8.png)

**Local Australian E8 Guides**
-   Microsoft Service Trust Portal has the local [Essential 8 guides](https://aka.ms/e8guides) - here you will find the documentation covering the following specifics (dated Nov 2023) 

-   [Microsoft General - Essential Eight - Application Hardening](https://learn.microsoft.com/en-us/compliance/anz/e8-app-harden)
- 	[Microsoft General - Essential Eight - Application Control](https://learn.microsoft.com/en-us/compliance/anz/e8-app-control)
-   [Microsoft General - Essential Eight - Multi-factor authentication](https://learn.microsoft.com/en-us/compliance/anz/e8-mfa)
- 	[Microsoft General - Essential Eight - Patch Applications](https://learn.microsoft.com/en-us/compliance/anz/e8-patch-app)
- 	[Microsoft General - Essential Eight - Patch Operating Systems](https://learn.microsoft.com/en-us/compliance/anz/e8-patch-os)
-   [Microsoft General - Essential Eight - Restrict administrative privileges](https://learn.microsoft.com/en-us/compliance/anz/e8-admin)
-   [Microsoft General - Essential Eight - Regular backups](https://learn.microsoft.com/en-us/compliance/anz/e8-backups)
-   [Microsoft General - Essential Eight - Restrict Microsoft Office macros](https://learn.microsoft.com/en-us/compliance/anz/e8-macro)

### **Hardening Guidance from ACSC**

-   [Hardening Microsoft Windows 10 and Windows 11 Workstations](https://www.cyber.gov.au/resources-business-and-government/maintaining-devices-and-systems/system-hardening-and-administration/system-hardening/hardening-microsoft-windows-10-and-windows-11-workstations)
-   [Hardening Microsoft 365, Office 2021, Office 2019 and Office 2016](https://www.cyber.gov.au/resources-business-and-government/maintaining-devices-and-systems/system-hardening-and-administration/system-hardening/hardening-microsoft-365-office-2021-office-2019-and-office-2016)
-   [Hardening Linux Workstations and Servers](https://www.cyber.gov.au/resources-business-and-government/maintaining-devices-and-systems/system-hardening-and-administration/system-hardening/hardening-linux-workstations-and-servers)





-   [Restricting Microsoft Office Macros](https://www.cyber.gov.au/resources-business-and-government/maintaining-devices-and-systems/system-hardening-and-administration/system-hardening/restricting-microsoft-office-macros)


### **Hardening Entra ID**

-   [Five steps to securing your identity infrastructure](https://learn.microsoft.com/en-us/azure/security/fundamentals/steps-secure-identity)
-   Also worth reviewing our Essential 8 guidance, especially MFA (aka.ms/e8guides)
-   Microsoft Azure **Identity Security Compass** - [Microsoft Security Best Practices](https://learn.microsoft.com/en-us/security/compass/compass)
-   Active Directory - [Best Practices for Securing Active Directory](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/plan/security-best-practices/best-practices-for-securing-active-directory)

### **AD onPrem**

A list of resources from DART perspective on Active Directory - courtesy
of Matt Zorich (X @reprise99)

-   BloodHound Edges
<https://bloodhound.readthedocs.io/en/latest/data-analysis/edges.html>
-   AD Security
<https://adsecurity.org/?page_id=4031>
-   [iRed Team](https://t.co/Y4BRxwdLu5) notes
[https://ired.team/offensive-security-experiments/active-directory-kerberos-abuse...](https://t.co/0w3Uo7TOSI)
-   SID History Persistence
[https://adsecurity.org/?p=1772](https://t.co/M7QX7w31Fw)
-   How AdminSdHolder & SDProp work
[https://techcommunity.microsoft.com/t5/ask-the-directory-services-team/five-common-questions-about-adminsdholder-and-sdprop/ba-p/396293...](https://t.co/5HPCBDnuZG)
-   Recovering from systemic identity compromise
[https://learn.microsoft.com/en-us/azure/security/fundamentals/recover-from-identity-compromise](https://t.co/Dfp1IWkS7z)
-   Abusing Active Directory ACLs/ACEs
[https://book.hacktricks.xyz/windows-hardening/active-directory-methodology/acl-persistence-abuse...](https://t.co/ZWUMlP58yv)
-   Defender for Identity Alerts Overview
[https://learn.microsoft.com/en-us/defender-for-identity/alerts-overview...](https://t.co/kkqqFsEB6i)
-   Best practices for securing AD
[https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/plan/security-best-practices/best-practices-for-securing-active-directory](https://t.co/a2suvfmpZm)
-   Mimikatz DCSync Abuse
[https://adsecurity.org/?p=1729](https://t.co/K51OQsXWSy)
-   Kerberoasting Overview
[https://ired.team/offensive-security-experiments/active-directory-kerberos-abuse/t1208-kerberoasting...](https://t.co/EqWNu84RoG)
-   Monitoring AD for signs of compromise
[https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/plan/security-best-practices/monitoring-active-directory-for-signs-of-compromise](https://t.co/enuOOAjAr1)

### **Identity**

-   Best Practices
<https://learn.microsoft.com/en-us/security/compass/compass>
-   From Jeffrey Appel
<https://jeffreyappel.nl/tips-for-preventing-against-new-modern-identity-attacks-aitm-mfa-fatigue-prt-oauth/>
    look at Partner section
-   MDCA (was MCAS) policies from AADIP P2 moving to D365 Console
    -   <https://learn.microsoft.com/en-us/microsoft-365/security/defender/microsoft-365-security-center-defender-cloud-apps?view=o365-worldwide&WT.mc_id=AZ-MVP-5004291#control>
    -   <https://www.linkedin.com/posts/sami-lamppu_microsoft-defender-for-cloud-apps-in-microsoft-activity-7011278821773471744-TcvX>?

### **Exchange Permissions check**

These two are subtly different, the first is on mailboxes, the second is
more focused on the Outlook Folders

-   <https://office365itpros.com/2020/03/16/exchange-online-mailbox-permissions/>
-    <https://github.com/12Knocksinna/Office365itpros/blob/master/ReportMailboxPermissionsMailboxes.PS1>
-   <https://office365itpros.com/2020/03/23/reporting-exchange-online-folder-permissions/>
-    <https://github.com/12Knocksinna/Office365itpros/blob/master/ReportPermissionsFolderLevel.PS1>
