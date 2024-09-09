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
<br />
3.On the right side, click on "Native SSH", then click "select"
<p align="center"> </p>
<img src="https://imgur.com/VDnBU86.png" height="80%" width="80%" >
<br />
<br />
4. Copy the Command
<p align="center"></p>
<img src="https://imgur.com/sQOFGPC.png" height="80%" width="80%" >
<br />
<br />
5. Open the Windows PowerShell and Run as Administrator, then paste the commmand in the terminal
<p align="center"> </p>
<img src="https://imgur.com/H6q2cQo.png" height="80%" width="80%" >
<br />
<br />
6. Replace the red arrow text with the path of ssh key file downloaded 
<p align="center"> </p>
<img src="https://imgur.com/TL5Ttwu.png" height="80%" width="80%" >
<br />
<br />
7. When login, want to check the distribution of Linux, run the following Command
<p align="center"> </p>
<img src="https://imgur.com/TEvagQb.png" height="80%" width="80%" >
<br />
<br />
8. The first thing is always to update the system first
<p align="center"></p>
<img src="https://imgur.com/iclgZgL.png" height="80%" width="80%" >
<br />
<br />
9. Now it comes to the fun part, install Fail2Ban on the machine   
<p align="center"></p>
<img src="https://imgur.com/Bi1sn6R.png" height="80%" width="80%" >
<br />
<br />
   
<p align="center">
Create Recource Group: <br/>
<img src="https://imgur.com/731vDl5.png" height="80%" width="80%" >
<br />
<br />
   
<p align="center">
Create Recource Group: <br/>
<img src="https://imgur.com/731vDl5.png" height="80%" width="80%" >
<br />
<br />
