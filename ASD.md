## **ASD Essential 8 (now ACSC)**
- [**Please start with this - ACSC Essential 8 – Health Report in Microsoft Sentinel**](https://techcommunity.microsoft.com/blog/microsoftsentinelblog/acsc-essential-8-%e2%80%93-health-report-in-microsoft-sentinel/3755702)
![](https://techcommunity.microsoft.com/t5/s/gxcuf89792/images/bS0zNzU1NzAyLTQ0NjUxNGkzM0RCODE5QjU4RjA2MEJB)

- [Essential 8 - ASD Site](https://www.cyber.gov.au/resources-business-and-government/essential-cyber-security/essential-eight)
- [Essential 8 - On a page](https://e8.jstuart.io)
- [Essential 8 - Mapping to ISM](https://www.cyber.gov.au/resources-business-and-government/essential-cyber-security/essential-eight/essential-eight-maturity-model-ism-mapping)
- [Microsoft's guidance on Essential 8 implementation](https://aka.ms/e8guides)
- [Collection of Australian M365 content on Essential 8](https://m365maps.com/australia.htm)
- [Microsoft Cybersecurity Reference Architecture](https://aka.ms/MCRA)
- [Australian IRAP](https://learn.microsoft.com/en-us/azure/compliance/offerings/offering-australia-irap)
- Licencing required to implment Essential 8 with Microsoft tooling
![](./images/Essential-8.png)

**Microsoft E8 Guides**
Microsoft has a [list of guides](https://aka.ms/e8guides) - focusing on each of the 8 Mitigation Strategies

- [Microsoft General - Essential Eight - Application Hardening](https://learn.microsoft.com/en-us/compliance/anz/e8-app-harden)

- [Microsoft General - Essential Eight - Application Control](https://learn.microsoft.com/en-us/compliance/anz/e8-app-control)

- [Microsoft General - Essential Eight - Multi-factor authentication](https://learn.microsoft.com/en-us/compliance/anz/e8-mfa)

- [Microsoft General - Essential Eight - Patch Applications](https://learn.microsoft.com/en-us/compliance/anz/e8-patch-app)

- [Microsoft General - Essential Eight - Patch Operating Systems](https://learn.microsoft.com/en-us/compliance/anz/e8-patch-os)

- [Microsoft General - Essential Eight - Restrict administrative privileges](https://learn.microsoft.com/en-us/compliance/anz/e8-admin)

- [Microsoft General - Essential Eight - Regular backups](https://learn.microsoft.com/en-us/compliance/anz/e8-backups)

- [Microsoft General - Essential Eight - Restrict Microsoft Office macros](https://learn.microsoft.com/en-us/compliance/anz/e8-macro)  

### **Hardening Guidance from ACSC**
- [Hardening Microsoft Windows 10 and Windows 11 Workstations](https://www.cyber.gov.au/resources-business-and-government/maintaining-devices-and-systems/system-hardening-and-administration/system-hardening/hardening-microsoft-windows-10-and-windows-11-workstations)

- [Hardening Microsoft 365, Office 2021, Office 2019 and Office 2016](https://www.cyber.gov.au/resources-business-and-government/maintaining-devices-and-systems/system-hardening-and-administration/system-hardening/hardening-microsoft-365-office-2021-office-2019-and-office-2016)

- [Hardening Linux Workstations and Servers](https://www.cyber.gov.au/resources-business-and-government/maintaining-devices-and-systems/system-hardening-and-administration/system-hardening/hardening-linux-workstations-and-servers)

### **Helpful Info/Links for each mitigation strategy**

#### Application Hardening

##### Notes

##### Links

- [Ad Block Tester](https://canyoublockit.com/) - This is reccomended by ACSC to test your ability to block ads. With the Manifest v3 changes, a combination of Browser Extensions and DNS blocking is required.
    - [uBlock Lite](https://chromewebstore.google.com/detail/ublock-origin-lite/ddkjiahejlhfcafbddmgiahcphecmpfh?hl=en)
    - [AdBlock Plus](https://chromewebstore.google.com/detail/adblock-plus-free-ad-bloc/cfhdojbkjhnklbpkdaibdccddilifddb?hl=en)
    - [NextDNS](https://nextdns.io/)
    - [Cisco Umbrella](https://umbrella.cisco.com/)

#### Application Control

##### Notes

- Applocker is required for E8 to control the execution of scripts in user profiles

- App Control for Business/Applocker only reports failure events to Advanced Hunting, Successful events are not logged. This can make it hard to find if a policy is working or not as you are looking for something that isn't there

- App Control for Business's Intelligent Security Graph is incompatible with Essential 8

- Microsoft isn't the only company that does App Control, If App Control for Business + AppLocker is to difficult to manage (It is a complicated/frustrating process, especially to start, even more so if you don't have your apps package). [Airlock](https://www.airlockdigital.com/) and [ThreatLocker](https://www.threatlocker.com/) are great alternatives  

##### Links

- [Deploy AppLocker via Intune](https://www.ccmtune.fr/2022/11/how-to-implement-applocker-with.html) - Good guide on how to deploy Applocker policies via Intune

- App Control for Business - [1](https://learn.microsoft.com/en-us/windows/security/application-security/application-control/app-control-for-business/appcontrol-and-applocker-overview) [2](https://patchmypc.com/wdac-intune) - Good doco on how App Control for Business works as well as deploying via Intune

- [~~WDAC~~ App Control for Business Wizard](https://webapp-wdac-wizard.azurewebsites.net/) - [Github](https://github.com/MicrosoftDocs/WDAC-Toolkit)

- [Querying App Control events centrally using Advanced hunting](https://learn.microsoft.com/en-us/windows/security/application-security/application-control/app-control-for-business/operations/querying-application-control-events-centrally-using-advanced-hunting) - Shows what the Action Types mean
	- App Control for Business Events = AppControl**CodeIntegrity** XYZ
	- AppLocker Events = **AppControl** XYZ

- [KQL for App Control Wizard](https://github.com/MicrosoftDocs/WDAC-Toolkit/blob/main/WDAC-Policy-Wizard/docs/using/advanced-hunting.md) - This Advanced Hunting query will get you the information you need for the App Control Wizard


#### Multi-factor authentication

#### Patch Applications

#### Patch Operating Systems

#### Restrict administrative privileges

#### Regular backups

#### Restrict Microsoft Office macros

- [ACSC's guide to disabling Macros](https://www.cyber.gov.au/resources-business-and-government/maintaining-devices-and-systems/system-hardening-and-administration/system-hardening/restricting-microsoft-office-macros) - Very good guide - Shows 6 different ways to set macro's, Along with the benefits/fritction. All these options can be set in Intune/GPO
- [Powershell Testing Scripts](https://github.com/JackStuart/Scripts/tree/main/Macros) - Scripts that you can run to confirm what settings are enabled are disabled, Easily customisable to whatever settings you want to test