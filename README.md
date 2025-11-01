# 🖥️ VMware Management Automation (PowerCLI)

> **PowerShell & PowerCLI automation scripts for VMware vSphere and ESXi environments**  
> Manage VMs, snapshots, and system health reports efficiently.  
> Tested on **Windows Server 2016+** and **PowerCLI 13+**

---

## 📋 Overview

This repository contains **PowerShell / PowerCLI** scripts for VMware administrators to automate daily vSphere operations, including:

- 🔧 **VM Management** — inventory, reporting, and power operations  
- 📸 **Snapshot Management** — create, list, and remove snapshots automatically  
- 📊 **vCenter / ESXi Health Reporting** — host, datastore, and snapshot usage reports  
- ⏰ **Scheduled Automation** — scripts designed to run unattended via Task Scheduler  

All scripts are modular and can be customized for your environment.

---

## 📁 Repository Structure

# 🖥️ VMware Management Automation (PowerCLI)

> **PowerShell & PowerCLI automation scripts for VMware vSphere and ESXi environments**  
> Manage VMs, snapshots, and system health reports efficiently.  
> Tested on **Windows Server 2016+** and **PowerCLI 13+**

---

## 📋 Overview

This repository contains **PowerShell / PowerCLI** scripts for VMware administrators to automate daily vSphere operations, including:

- 🔧 **VM Management** — inventory, reporting, and power operations  
- 📸 **Snapshot Management** — create, list, and remove snapshots automatically  
- 📊 **vCenter / ESXi Health Reporting** — host, datastore, and snapshot usage reports  
- ⏰ **Scheduled Automation** — scripts designed to run unattended via Task Scheduler  

All scripts are modular and can be customized for your environment.

---

## 📁 Repository Structure

📦 vmware-automation
┣ 📜 Connect-vCenter.ps1 # Connects to vCenter using credentials
┣ 📜 Get-VMInventory.ps1 # Generates VM inventory report
┣ 📜 Manage-Snapshots.ps1 # Create, list, and cleanup snapshots
┣ 📜 Get-ESXiHealthReport.ps1 # Reports host and datastore usage
┣ 📜 VMware-Automation.psm1 # (Optional) PowerShell module for all functions
┣ 📜 Schedule-Automation.ps1 # Example for daily scheduled tasks
┗ 📄 README.md # Documentation (you are here)


## ⚙️ Prerequisites

- **Windows Server 2016 or later**
- **PowerShell 5.1+** or **PowerShell 7.x**
- **VMware PowerCLI** module  
  ```powershell
  Install-Module -Name VMware.PowerCLI -Scope CurrentUser
  Set-PowerCLIConfiguration -Scope User -ParticipateCEIP $false -InvalidCertificateAction Ignore -Confirm:$false
