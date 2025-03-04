# **Noa Linux**  
**Be free. Everything is right in front of you.**  

## **Overview**  
Noa Linux is a lightweight and flexible Linux distribution that adopts the **Noa Package Manager** as both its package management system and init system.  

**Noa Linux is designed for CUI (Character User Interface) environments and does not support GUI.**  

## **Key Features**  

### **1. Noa Package Manager (Also Functions as an Init System)**  
Noa Linux uses the **Noa Package Manager** as its default package manager and init system.  

- **Boot Process**  
  - The system starts using the `noa boot start` command.  
  - This allows Noa Package Manager to function as the init system and manage processes.  

- **Package Management**  
  - **Source-based Package Installation**  
    - Packages are built from source code.  
    - This allows for system optimization and a high degree of customization.  

  - **Binary Package Support (nover)**  
    - For users who cannot compile packages or prefer faster installations, Noa Linux will offer a binary package system called **nover** (currently in development).  

### **2. Recovery Mode (Automated System Repair)**  
To maintain system integrity, Noa Linux verifies the **BLAKE3 hash** of critical files at boot time.  

- **If Corruption or Unauthorized Modifications Are Detected**  
  - The system automatically enters **Recovery Mode**.  
  - A minimal environment is launched, instructing the user to reinstall Noa.  
  - After successful reinstallation, a reboot restores the system to normal operation.  

- **Init System During Recovery (runit)**  
  - Noa Linux primarily uses **Noa init**, but in **Recovery Mode**, it switches to **runit** as the init system.  
  - This ensures a minimal and stable environment for system recovery.  

## **Current Development Status**  
- Noa Package Manager is under development.  
- The nover binary package system is being designed.  
- Recovery Mode is in the planning phase.  

This document will be updated as development progresses.
