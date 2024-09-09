# Secure-Linux-Server-with-Fail2Ban
This Repository is about securing Linux Server with Fail2Ban, it will not 100% block the attack, but it will add a layer of security to defend the Server

- [Introduction](https://github.com/TayLuo/Secure-Linux-Server-with-Fail2Ban/blob/main/Introduction%20to%20Fail2Ban)
- [Skills and Knowledge gained](https://github.com/TayLuo/Secure-Linux-Server-with-Fail2Ban/blob/main/Skills%20and%20Knowledge%20Gained)

The Following are the step by step guide on how to install and configure Fail2Ban:

In this project I used [Azure](https://azure.microsoft.com/en-us/get-started/azure-portal) for my project, you can choose whichever you prefer. 
1. The first step is to set up a Linux VM in azure, I will not show you step by step how to set up a VM, if you need help, please check out
   [here](https://learn.microsoft.com/en-us/azure/virtual-machines/linux/quick-create-portal?tabs=ubuntu)
2. After successfully created and deployed the VM, there will be a public IP address given to you.
   <p align="center"> </p> 
<img src="https://imgur.com/WUOvJwq.png" height="80%" width="80%" >
<br />
3.On the right side, click on "Native SSH", then click "select"
<p align="center"> </p>
<img src="https://imgur.com/VDnBU86.png" height="80%" width="80%" >
<br />
4. Copy the Command
<p align="center"></p>
<img src="https://imgur.com/sQOFGPC.png" height="80%" width="80%" >
<br />
5. Open the Windows PowerShell and Run as Administrator, then paste the commmand in the terminal
<p align="center"> </p>
<img src="https://imgur.com/H6q2cQo.png" height="80%" width="80%" >
<br />
6. Replace the red arrow text with the path of ssh key file downloaded 
<p align="center"> </p>
<img src="https://imgur.com/TL5Ttwu.png" height="80%" width="80%" >
<br />
7. When login, want to check the distribution of Linux, run the following Command
<p align="center"> </p>
<img src="https://imgur.com/TEvagQb.png" height="80%" width="80%" >
<br />
8. The first thing is always to update the system first
<p align="center"></p>
<img src="https://imgur.com/iclgZgL.png" height="80%" width="80%" >
<br />
9. Now it comes to the fun part, install Fail2Ban on the machine   
<p align="center"></p>
<img src="https://imgur.com/Bi1sn6R.png" height="80%" width="80%" >
<br />
10. Let's start the service and check the status of the service  
<p align="center"> </p>
<img src="https://imgur.com/jdkaYom.png" height="80%" width="80%" >
<br />
<p align="center"></p>
<img src="https://imgur.com/PpQo71U.png" height="80%" width="80%" >
<br />
<p align="center"></p>
<img src="https://imgur.com/qAAOrNr.png" height="80%" width="80%" >
<br />
11. It is always to copy the file you are going to configure first, just in case.   
<p align="center"></p>
<img src="https://imgur.com/tfKpk8v.png" height="80%" width="80%" >
<br />
12. Check if the file is copied
<p align="center"></p>
<img src="https://imgur.com/YcCkBCW.png" height="80%" width="80%" >
<br />
13. Let's do some fun things by configure the file using "vi" editor
<p align="center"></p>
<img src="https://imgur.com/3SkUQym.png" height="80%" width="80%" >
<br />
14. When get into the configuration file, uncomment the line with "ignore IP" and add "127.0.0.1" and "Your public IP"
<p align="center"></p>
<img src="https://imgur.com/7wSDVRO.png" height="80%" width="80%" >
<br />
15. Regarding how long you want to ban the unknown IP, how many times can an IP try to access, it is up to the organization
<p align="center"> </p>
<img src="https://imgur.com/ErfAsPt.png" height="80%" width="80%" >
<br />
16. There is one option, the email coulb be sent if there is an IP trying to access the Server
<p align="center"></p>
<img src="https://imgur.com/dc16UKl.png" height="80%" width="80%" >
<br />
17. Under SSHD section, add the following line 
<p align="center"></p>
<img src="https://imgur.com/03fOZJe.png" height="80%" width="80%" >
<br />
18. Once you're satified with the settings, restart the fail2ban service
<br />
19. What banning looks like
<p align="center"> </p>
<img src="https://imgur.com/NBzTzKe.png" height="80%" width="80%" >
<br />
20. If an legit IP got banned from accessing your Server, here is how to unban an IP
<p align="center"></p>
<img src="https://imgur.com/z7SuQr2.png" height="80%" width="80%" >
<br />
<br />

Feel free to explore the repository and follow the included instructions to replicate the setup on your own Linux server. 
Your feedback and contributions are always welcome!
