# Open-Vas-Lab

<h2>Description</h2>
During this scan, the OpenVAS vulnerability scanner was used. The following will include the necessary steps to scan target devices, such as Windows machines & Linux machines. OpenVAS can be manually installed and is recommended, however, the screenshots below will showcase a cloud virtual machine environment that already has OpenVAS installed. There are two virtual machine targets that we will be scanning.
<br />



<h2>Environments Used </h2>

- <b>Windows XP </b> 
- <b>Linux</b>

<h2>Tool Used </h2>
- <b> OpenVAS
<h2>IMPORTANT NOTE!</h2>
For security reasons, IP addresses and other sensitive information in screenshots have been blurred out. 

<h2>Lab walk-through:</h2>

<h2>Screenshot 1:</h2>
<div class="step">
  <p>Step 1:<br>
  Before we start up OpenVAS, ensure your target machines are running and are discoverable. As shown below, the Windows XP and Linux machine are started up. With the command "netdiscover -I br0 -l" the IP addresses can be shown.</p>
  <img src="https://i.imgur.com/moxoGai.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>

<h2>Screenshot 2:</h2>
<div class="step">
  <p>Step 2:<br>
  Now click gvm start in your Linux machine that you will be performing the scan on.</p>
  <img src="https://i.imgur.com/4MOgCq4.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>


<h2>Screenshot 3:</h2>
<div class="step">
  <p>Step 3:<br>
  You should be given an address which you can see is highlighted below. You want to copy and paste this URL into Firefox.</p>
  <img src="https://i.imgur.com/9aKbqW9.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>

  
<h2>Screenshot 4:</h2>
<div class="step">
  <p>Step 4:<br>
Type in your credentials and login.</p>
<img src="https://i.imgur.com/paONDdN.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>

 
<h2>Screenshot 5:</h2>
<div class="step">
  <p>Step 5:<br>
Under the scans tab, click on the wang icon and then Task Wizard. 
</p>
<img src="https://i.imgur.com/AH3fncy.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>
  
<h2>Screenshot 6:</h2>
<div class="step">
 <p>Step 6:<br>
Once the task wizard panel pops up, this is where you type in the IP address of your first machine target. Here below the Windows Machine IP address was targeted. After entering your first machine's IP address, click start scan. 
</p>
<img src="https://i.imgur.com/BFyZ0qj.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>

<h2>Screenshot 7:</h2>
<div class="step">
 <p>Step 7:<br>
Keep in mind, if you are using a cloud environment like I am, the scan will take very long. As you can see below the scan has started and the status bar will show the progress. 
</p>
<img src="https://i.imgur.com/sI53NPt.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>

<h2>Screenshot 8:</h2>
<div class="step">
 <p>Step 8:<br>
While your 1st machine is scanning, you can choose to go back and also start the scan for the 2nd machine which is shown here below. 
</p>
<img src="https://i.imgur.com/5lHhu61.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>


<h2>Screenshot 9:</h2>
<div class="step">
<p>Step 9:<br>
After your first machine finishes scanning, click on the report. Here, we can see the results and the different tabs that we will be looking at. 
</p>
<img src="https://i.imgur.com/qdhYcc9.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>

<h2>Screenshot 10:</h2>
<div class="step">
<p>Step 10:<br>
Below showcases the results, vulnerabilities, and how high the severity of the weaknesses that are on the host. Analyze and record how many vulnerabilities are reported, as well as the severity of each one. 
</p>
<img src="https://i.imgur.com/cYqNuKZ.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>

<h2>Screenshot 11:</h2>
<div class="step">
<p>Step 11:<br>
Clicking on the "OS End of Life Detection" vulnerability above, we can see a description of the vulnerability and can read the details of what hackers might do to exploit this and a solution as well. 
</p>
<img src="https://i.imgur.com/G7FzNuj.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>

<h2>Screenshot 12:</h2>
<div class="step">
<p>Step 12:<br>
Click on each of the tabs to analyze the results and different cases. Here below reports that a security update is missing and can be exploited by buffer overflow. When using this scan, it is important to understand that these vulnerabilities are accurate and that the solutions are highly considered. 
</p>
<img src="https://i.imgur.com/W5Fs5Xk.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>

<h2>Screenshot 13:</h2>
<div class="step">
<p>Step 13:<br>
Again, view the different tabs and click on each case. Below we see that there are multiple different OS vulnerabilities relevant and that this machine could be vulnerable to denial of service attacks. Notice how just by not keeping software up to date, the system could be exploited. 
</p>
<img src="https://i.imgur.com/j8YWv6c.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>

<h2>Step 14:</h2>
<div class="step">
<p>Step 14:<br>
After carefully reading through the results and descriptions of each case, repeat steps 10-13 with your 2nd machine after the scan completes. 
</p>
<img src="https://i.imgur.com/BFyZ0qj.png" height="80%" width="80%" alt="Disk Sanitization Steps">
</div>

<h2> OS End Of Life Detection:</h2>
<p>
The security risk of running this software is that it is no longer supported and the security fixes that would normally protect users from known vulnerabilities won't be provided. Instead, hackers will discover these risks which are usually known to the public, and exploit them with no patch to protect the users against those risks. Organizations will somewhere down the line depend on EOL Operating Systems because the process of migrating to new Operating Systems constantly creates challenges. Although that might be the case, there are extended support vendors at a price that will support Operating Systems that are no longer supported. The best way to prevent this though is to always schedule mandatory updates and patches for Operating Systems. 
</p>


<h2>SMB NTLM: </h2>
<p>
The OpenVAS report explains that the NTLM cryptography scheme is outdated and during SMB authentication, can be easily bypassed by hackers. A solution to this would be to implement Digital Certificate Authentication. This will ensure users never send their authentication information to the wrong SSID. This process involves a cryptographic handshake with a RADIUS server and user device. 
</p>

<h2>SMB remote code execution: </h2>
<p>
OpenVAS states that the exploitation of SMB packets will allow remote unauthenticated attackers to cause denying the service, by sending crafted network messages to the systme. Currently, ARM64, Windows32 and 64-bit editions, Windows 10(1903 & 1909), and Windows Serer (versions 1903 & 1909) are affected. One solution to this problem is to disable compression using the powershell command: 
- "Set-ItemProperty -Path "HKLM:\SYSTEM\CurrentControlSet\Services\LanmanServer\Parameters” DisableCompression -Type DWORD -Value 1 –Force". 
Another solution would be to block the TCP port 445 to stop malicious code on firewall. It's recommended to update to Windows 11. 
</p>

<h2>SMBv1: </h2>
<p>
Successful exploitation would allow remote attackers to gain the ability to execute code on the target server. This could lead to information disclosure from the server. Interestingly, an article I found for a solution explains the steps to exploit this vulnerability. Basically, SMBv1 can be disabled at any time and if it is still being used, should install patches. 
</p>
  
