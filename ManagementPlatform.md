| Service                         | Functionality                                                                              | Commercial | GCC | GCC High  | DoD       | Notes                                                                                                                                                                                                                                                                                                               | Source                                                                                                                                                                                                 |
|---------------------------------|--------------------------------------------------------------------------------------------|------------|-----|-----------|-----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Azure AD                        | Login through the Web                                                                      | Yes        | Yes | Yes       | Yes       |                                                                                                                                                                                                                                                                                                                     |                                                                                                                                                                                                        |
| Azure AD                        | Login through external Identity Provider                                                   | Yes        | Yes | See Notes | See Notes | ADFS is the only supported external IdP                                                                                                                                                                                                                                                                             |                                                                                                                                                                                                        |
| Azure AD                        | Federated Logon                                                                            | Yes        | Yes | See Notes | See Notes | ADFS may require whitelisting server addresses                                                                                                                                                                                                                                                                      |                                                                                                                                                                                                        |
| Azure AD                        | B2B Collaboration                                                                          | Yes        | Yes | See Notes | See Notes | B2B collobation only between Government tenants and Microsoft or Google Accounts                                                                                                                                                                                                                                    | https://docs\.microsoft\.com/en\-us/azure/active\-directory/external\-identities/current\-limitations\#how\-can\-i\-tell\-if\-b2b\-collaboration\-is\-available\-in\-my\-azure\-us\-government\-tenant |
| Azure AD                        | B2B Colloboration through Power BI                                                         | Yes        | Yes | No        | No        | When you invite a guest user from within Power BI, the B2B flow is not used and the guest user won't appear in the tenant's user list\. If a guest user is invited through other means, they'll appear in the Power BI user list, but any sharing request to the user will fail and display a 403 Forbidden error\. | https://docs\.microsoft\.com/en\-us/azure/azure\-government/compare\-azure\-government\-global\-azure\#azure\-active\-directory\-premium\-p1\-and\-p2                                                  |
| Azure AD                        | Office 365 Groups \- Internal                                                              | Yes        | Yes | Yes       | Yes       |                                                                                                                                                                                                                                                                                                                     |                                                                                                                                                                                                        |
| Azure AD                        | Office 365 Groups \- Shared                                                                | Yes        |     | No        | No        | Office 365 Groups are not supported for B2B users and can't be enabled\.                                                                                                                                                                                                                                            | https://docs\.microsoft\.com/en\-us/azure/azure\-government/compare\-azure\-government\-global\-azure\#azure\-active\-directory\-premium\-p1\-and\-p2                                                  |
| Azure AD                        | Hardware OATH Tokens                                                                       | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/azure/azure\-government/compare\-azure\-government\-global\-azure\#azure\-active\-directory\-premium\-p1\-and\-p2                                                  |
| Azure AD                        | Trusted Ips                                                                                | Yes        |     | No        | No        | Named Locations required \- fully functional workaround                                                                                                                                                                                                                                                             | https://docs\.microsoft\.com/en\-us/azure/azure\-government/compare\-azure\-government\-global\-azure\#azure\-active\-directory\-premium\-p1\-and\-p2                                                  |
| Azure AD                        | Enterprise State Roaming                                                                   | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/azure/azure\-government/compare\-azure\-government\-global\-azure\#azure\-active\-directory\-premium\-p1\-and\-p2                                                  |
| Enterprise Mobility \+ Security | Intune Standalone Deployments                                                              | Yes        | Yes | Yes       | Yes       |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-intune\-govt\-service\-description                                                                                   |
| Enterprise Mobility \+ Security | Legacy PC \(Windows 7 and 8\) Management                                                   | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-intune\-govt\-service\-description                                                                                   |
| Enterprise Mobility \+ Security | Windows 10 PC Management                                                                   | Yes        | Yes | Yes       | Yes       |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-intune\-govt\-service\-description                                                                                   |
| Enterprise Mobility \+ Security | Exchange Connector                                                                         | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-intune\-govt\-service\-description                                                                                   |
| Enterprise Mobility \+ Security | SCCM Co\-Management                                                                        | Yes        |     | See Notes | See Notes | Requires 1906 or Later                                                                                                                                                                                                                                                                                              | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-intune\-govt\-service\-description                                                                                   |
| Enterprise Mobility \+ Security | Windows Autopilot                                                                          | Yes        |     | No        | No        | Planning is underway                                                                                                                                                                                                                                                                                                | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-intune\-govt\-service\-description                                                                                   |
| Enterprise Mobility \+ Security | Microsoft Business Store                                                                   | Yes        |     | No        | No        | Planning is underway                                                                                                                                                                                                                                                                                                | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-intune\-govt\-service\-description                                                                                   |
| Enterprise Mobility \+ Security | Jamf Pro Integration                                                                       | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-intune\-govt\-service\-description                                                                                   |
| Enterprise Mobility \+ Security | Mobile Threat Defense                                                                      | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-intune\-govt\-service\-description                                                                                   |
| Enterprise Mobility \+ Security | Windows Defender ATP Threat Analytics                                                      | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-intune\-govt\-service\-description                                                                                   |
| Microsoft Defender ATP          | Threat & Vulnerability Management                                                          | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Automated Investigation and Remediation                                                    | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Response to Office 365 Alerts                                                              | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Live Response                                                                              | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Threat Protection Report                                                                   | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Device Health and Compliance Report                                                        | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | 3rd Party Integrations                                                                     | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Email Notifications                                                                        | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Azure ATP Integration                                                                      | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Azure Information Protection Integration                                                   | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Office 365 Advanced Threat Protection Integration                                          | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Microsoft Cloud App Security Integration                                                   | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Skype for Business Integration                                                             | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Microsoft Intune Integration                                                               | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Windows Defender ATP Linux Support                                                         | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Microsoft Defender ATP          | Windows Defender ATP macOS Support                                                         | Yes        |     | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/windows/security/threat\-protection/microsoft\-defender\-atp/commercial\-gov                                                                                       |
| Azure Information Protection    | Document Tracking and Revocation                                                           | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-aip\-premium\-govt\-service\-description                                                                             |
| Azure Information Protection    | Classification Add In for Office                                                           | Yes        | Yes | See Notes | See Notes | Requires Microsoft 365 Apps\. Does not support Office 2010 \- 2016                                                                                                                                                                                                                                                  | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-aip\-premium\-govt\-service\-description                                                                             |
| Azure Information Protection    | IRM Add In for Office                                                                      | Yes        | Yes | See Notes | See Notes | Requires Microsoft 365 Apps\. Does not support Office 2010 \- 2016                                                                                                                                                                                                                                                  | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-aip\-premium\-govt\-service\-description                                                                             |
| Azure Information Protection    | Sharing Protected Documents to Commercial                                                  | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-aip\-premium\-govt\-service\-description                                                                             |
| Azure Information Protection    | IRM for SharePoint Online                                                                  | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-aip\-premium\-govt\-service\-description                                                                             |
| Azure Information Protection    | Rights Management Connector                                                                | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-aip\-premium\-govt\-service\-description                                                                             |
| Azure Information Protection    | AD RMS Mobile Device Extenstion                                                            | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-aip\-premium\-govt\-service\-description                                                                             |
| Cloud App Security              | API connector for AWS GovCloud                                                             | No         | No  | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-cloud\-app\-security\-govt\-service\-description                                                                     |
| Cloud App Security              | API connector for public clouds                                                            | Yes        | Yes | Yes       | Yes       |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-cloud\-app\-security\-govt\-service\-description                                                                     |
| Cloud App Security              | Content Inspection                                                                         | Yes        | Yes | Yes       | Yes       |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-cloud\-app\-security\-govt\-service\-description                                                                     |
| Cloud App Security              | Microsoft Information Protection Labels                                                    | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-cloud\-app\-security\-govt\-service\-description                                                                     |
| Cloud App Security              | Conditional Access app control                                                             | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-cloud\-app\-security\-govt\-service\-description                                                                     |
| Cloud App Security              | Admin Email Notifications                                                                  | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-cloud\-app\-security\-govt\-service\-description                                                                     |
| Cloud App Security              | AWS Security Configuration Assessments                                                     | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-cloud\-app\-security\-govt\-service\-description                                                                     |
| Cloud App Security              | Azure Sentinel integration                                                                 | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-cloud\-app\-security\-govt\-service\-description                                                                     |
| Cloud App Security              | Microsoft Defender ATP Integration                                                         | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-cloud\-app\-security\-govt\-service\-description                                                                     |
| Cloud App Security              | Surfacing Microsoft Cloud App Security controls in Microsoft Secure Score                  | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-cloud\-app\-security\-govt\-service\-description                                                                     |
| Azure ATP                       | Integration with Microsoft Defender Advanced Threat Protection \(Microsoft Defender ATP\)  | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-azure\-atp\-govt\-service\-description                                                                               |
| Azure ATP                       | VPN integration, offering the ability to collect accounting information from VPN solutions | Yes        | Yes | No        | No        |                                                                                                                                                                                                                                                                                                                     | https://docs\.microsoft\.com/en\-us/enterprise\-mobility\-security/solutions/ems\-azure\-atp\-govt\-service\-description                                                                               |