# LilBestie-Server-Manual
Lil Bestie is my personal homelab server. She contains multitudes, this is her manual. 
Lil Bestie begain life as a Windows 10 home server, until an unfortunate encounter with a hacker left her hobbled. 

As the dedicated systems engineer, I confidently told the cats, "Ladies, we can rebuild her." 

🚀 USS Lil Bestie
=================
<img width="2576" height="2184" alt="chrome_Z8yt4ydHDs" src="https://github.com/user-attachments/assets/c84a9b90-6451-4a82-9fa1-b1f079f0c202" />

Captain’s Log – Commissioning Record
------------------------------------

**Vessel Name:** Lil Bestie
**Call Sign:** multiplexer
**IP Address:** 192.168.1.157
**OS:** Debian 13 (Trixie)
**Primary Engineer:** Michelle
**Original State:** Windows 10, dead in the water

Architecture Diagram
--------------------
Internet
   |
Router (DHCP reservation)
   |
multiplexer (Debian 13)
   ├── Emby (8096)
   ├── Portainer (9443)
   ├── Homarr (7575)
   ├── Dashdot (3002)
   ├── Caddy (8080)
   └── Samba (/srv/storage)

Stardate: The Week™
-------------------

Initial assessment revealed:

*   Windows 10 incapable of updating
    
*   Hardware deemed “unsupported”
    
*   Ransomware damage previously sustained
    
*   RAID configuration unknown
    
*   Boot instability
    
*   Kernel drama
    
*   Network instability
    
*   Emotional instability (briefly)
    

Decision made to scuttle legacy system and rebuild from bare metal.

Phase I – Resurrection
----------------------

*   RAID 6 confirmed on LSI MegaRAID 9271-8i
    
*   Debian installed on NVMe
    
*   XFS RAID mounted at /srv/storage
    
*   Kernel regressions identified and defeated
    
*   Stable kernel achieved: 6.12.73+deb13-amd64
    
*   Boot restored
    
*   systemd appeased
    

The vessel breathed again.

Phase II – Infrastructure Online
--------------------------------

The following systems are operational:

### 🐳 Container Subsystem (Docker)

*   Status verified via docker ps
    
*   Persistent restart policies enabled
    

### 🎬 Emby Media Service

*   Streaming operational
    
*   Media mounted from /srv/storage/media
    

### 🛠 Portainer Control Console

*   Administrative access secured
    
*   HTTPS functional
    

### 🌐 Web Hosting (Caddy)

*   Personal site deployed
    
*   Inside jokes embedded
    
*   Romantic infrastructure confirmed
    

### 📂 Samba File Transport

*   \\\\192.168.1.157\\Media
    
*   Mapped as Drive Z:
    
*   Basement USB exile officially ended
    

### 🖥 Homarr Command Dashboard

*   Centralized control interface operational
    
*   Widgets online
    
*   Empire view achieved
    

Phase III – Stabilization
-------------------------

*   DHCP reservation configured
    
*   Network route verified
    
*   /srv/storage mount hardened with:
    
    *   nofail
        
    *   x-systemd.automount
        
*   Reboot survivability confirmed
    
*   Post-reboot validation checklist established
    

The vessel now boots reliably without ritual sacrifice.

Phase IV – Data Preservation Protocol
-------------------------------------

Critical assets identified:

*   Photos
    
*   Recipes
    
*   Minecraft worlds
    
*   Website content
    

Backup strategy in progress:

*   Primary: RAID array
    
*   Secondary: 8TB backup disk
    
*   Automation via cron + rsync
    
*   Volume snapshotting for Docker
    

Ransomware shall not pass again.

Current Operational Checklist
-----------------------------

After reboot, confirm:

`   uname -r  df -h | grep storage  docker ps   `

If all systems green → vessel stable.

Known Victories
---------------

*   Kernel regression defeated
    
*   Mount failure corrected
    
*   Network cable reseated (twice)
    
*   Docker revived
    
*   Port confusion resolved
    
*   Samba typo conquered
    
*   Homarr image source corrected
    
*   WD40 joke deployed successfully
    

Crew Notes
----------

Primary Engineer reports increased affection for:

*   Command line interfaces
    
*   Text-based configuration
    
*   Immutable infrastructure
    
*   Norse-named dashboards
    

Morale currently high.

Prince has been played.

Cookies have been consumed.

Future Mission Objectives
-------------------------

*   Automated backup verification
    
*   Minecraft server deployment
    
*   Reverse proxy refinement
    
*   Health telemetry page
    
*   Git-tracked infrastructure
    
*   Optional: next-level chaos engineering
    
Lessons Learned
---------------
*  Linux > Windows for a zombie machine with vintage hardware, but life left in her
  
*  Persistence pays off
  
*  Always code with cats and/or cookies
  
*  Nothing says "I love you" like a server
  
*  A sense of humor is the most valuable tool in an engineer's toolbox

What I'd Do Differently
-----------------------
*  Give up on Windows faster
  
*  Containerized critical services sooner
  
*  Created a better backup before all this happened. 

Commissioning Statement
-----------------------

USS Lil Bestie has been fully recommissioned from defunct Windows relic to stable Debian infrastructure platform.

All core systems functional.All services operational.All romance containerized.

Signed,**Captain Michelle**Automation EngineerBreaker of KernelsMapper of Z Drives
