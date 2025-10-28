\# el-guero-i2p



This repository documents my personal \*\*I2P eepsite\*\* setup.

<img width="1024" height="768" alt="image" src="https://github.com/user-attachments/assets/69865fd1-63be-4714-9b6e-bb2e358441a1" />

---

\## Overview

This eepsite hosts a mirror of my GitHub Pages site inside the \*\*I2P network\*\*.



\*\*I2P Address:\*\*  

http://gvbv6vo7gcgwy24spe7hfhqc4v7cub2zxrriza2cuuspyymi6dba.b32.i2p



Accessible only via the I2P browser or any browser configured with the I2P HTTP proxy.



---



\## How It Works



\- Eepsite files live here:  

&nbsp; `C:\\Users\\David\\AppData\\Local\\i2p\\eepsite\\docroot`



\- The content is mirrored from:  

&nbsp; `C:\\Users\\David\\david-marin-0xff.github.io`



\- The I2P router console is at:  

&nbsp; `http://127.0.0.1:7658/`



My eepsite becomes reachable \*\*only while the I2P router is running\*\*.



---



\## How to Start the Site



1\. I launch I2P.  

2\. Wait until tunnels are ready (“I2P is ready”).  

3\. My eepsite is instantly reachable.



If I turn off my PC or close I2P, the site goes \*\*offline\*\*.  

Restart I2P and it comes \*\*back online\*\* automatically.



---



\## Sync GitHub Pages → Eepsite



To update my local eepsite with your latest GitHub Pages content:



```powershell

robocopy "C:\\Users\\David\\david-marin-0xff.github.io" "C:\\Users\\David\\AppData\\Local\\i2p\\eepsite\\docroot" /E /COPYALL /R:2 /W:2 /XA:SH /XF "eepsite.key" "i2pkeys.dat" "router.keys"

```



---



\## Personal Notes to remember:



\- Don’t delete or overwrite `eepsite.key`.  

\- Enable \*\*“Auto Start Tunnel”\*\* in the I2P Hidden Service Manager.  

\- Keep your I2P router updated for better stability.



---



