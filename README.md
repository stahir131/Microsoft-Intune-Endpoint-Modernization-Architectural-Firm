### Microsoft Intune & Endpoint Modernization — Architectural Firm

I recently led the endpoint modernization and **Microsoft Intune migration** for an architectural firm transitioning away from a traditional on-premises environment.

The client’s existing infrastructure relied on an on-premises Windows Server providing **Active Directory, Print Services, and Microsoft Entra ID synchronization (ADSync)**. The objective was to modernize endpoint management, reduce dependency on on-premises infrastructure, improve security and application delivery, and ultimately decommission the legacy server while minimizing disruption to users.

#### Environment Assessment & Migration Planning

I began with an assessment of the existing environment to identify dependencies, applications, device requirements, and potential migration risks. Because the firm relies heavily on specialized architectural and engineering software, particular attention was given to application compatibility, deployment methods, installation requirements, and user impact.

The migration strategy was designed around a controlled transition rather than a “big bang” approach, allowing core applications and security configurations to be validated before moving users and devices into the new management platform.

#### Intune Architecture & Endpoint Configuration

I designed and configured the new **Microsoft Intune environment**, including:

* Windows enrollment profiles
* Device configuration policies
* Compliance policies
* Endpoint security policies
* BitLocker disk encryption
* Application deployment and management
* Microsoft Entra ID integration
* Windows Autopilot hardware registration
* Security and endpoint management baselines

PowerShell automation was used to collect **Windows hardware IDs** from existing devices and prepare them for Intune enrollment. The hardware information was exported and imported into Intune ahead of the migration, allowing devices to be prepared before the transition.

A Windows reset process was then deployed to the existing endpoints. Once the reset was completed, users could sign in and begin the enrollment process, transitioning the devices from the legacy management model into the new cloud-managed environment.

#### Enterprise Application Packaging & Deployment

Application management was one of the most significant components of the project due to the firm's dependence on Autodesk and other resource-intensive applications.

Approximately **50 Windows applications were packaged and published through Intune**, providing centralized application lifecycle management and a self-service experience through the Microsoft Company Portal.

Key applications included:

* Autodesk Revit 2024, 2025, 2026 & 2027
* AutoCAD
* Autodesk Desktop Connector
* Autodesk ReCap Pro
* Autodesk Content Catalog
* Navisworks Manage
* Adobe Creative Cloud
* Bluebeam Revu
* Cisco VPN Client
* Endpoint security/antivirus software
* Various architectural and engineering add-ons

Applications were strategically assigned based on business requirements. Frequently required applications were deployed automatically as **Required applications**, while larger or less frequently used applications were made available through **Company Portal**.

This approach reduced unnecessary deployment overhead while giving users flexibility to install resource-intensive applications when needed.

#### Cloud-Based Print Infrastructure

As part of the infrastructure modernization, the legacy print server was also migrated to **Printix**, moving print management away from the on-premises domain controller.

The new cloud-based print architecture eliminated the need for a dedicated print server and reduced the firm's dependency on on-premises infrastructure while providing centralized cloud-based printer management.

#### Project Outcome

The project successfully transitioned the firm's Windows endpoint management from a traditional on-premises model to a **cloud-managed Microsoft Intune environment**.

Key outcomes included:

* Modernized Windows endpoint management
* Centralized application deployment through Intune
* Self-service application installation through Company Portal
* Automated Windows hardware registration
* Standardized security and compliance policies
* BitLocker encryption management
* Reduced dependency on on-premises infrastructure
* Cloud-based print management through Printix
* Improved scalability for future device deployments
* Reduced administrative overhead associated with traditional domain-based management

Following successful migration and validation, the legacy on-premises server was **decommissioned and shut down**, completing the transition toward a modern cloud-managed endpoint environment.

This project strengthened my experience in **Microsoft Intune architecture, endpoint modernization, PowerShell automation, application packaging, Windows migration strategy, security configuration, and cloud transformation**, while balancing technical requirements with the operational needs of a specialized architectural organization.
