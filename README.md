<p align="center">
<img src="images/adds-column-header.png" alt="Azure active Directory Domain Service"  />
</p>

<h1>Basic Azure AD Domain Services and VM Joining Setup.</h1>
Azure Active Directory Domain Services (Azure AD DS) provides managed domain services such as domain join, group policy, LDAP, Kerberos/NTLM authentication that is fully compatible with Windows Server Active Directory. The integration lets users sign in using their corporate credentials, and you can use existing groups and user accounts to secure access to resources.. <br />


<h2>Prerequisites and Technologies Used</h2>

- An active Azure subscription
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Virtual Machine with DNS Server
- Various Command-Line Tools
- Various Network Protocols ( RDH, DNS, )

<h2>Operating Systems Used </h2>
- Windows 10 (21H2)
- Windows Server 2022

<h2>Actions and Observations</h2>
<h2>High-Level Steps</h2>

<b>- Step 1:</b>
From Microsoft Azure porta, Search for <b>Azure AD Domain Services</b> and click on the search result <b>Azure AD Domain Services</b>.
<p>
<img src="images/AD-1.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<b>- Step 2:</b>
Click on the Create Azure AD Domain Services button on the Azure AD Domain Services window.
<p>
<img src="images/ad2-1.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<b>- Step 3:</b>
Now select the Azure Subscription and the Resource group. Select your DNS domain name as your wish then Click on Next.
<p>
<img src="images/AD-2.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<b>- Step 4:</b>
In the Networking window, Select the Virtual Network and Subnet, or we can create a new Virtual Network as your wish for your managed domain. Then click Next.
<p>
<img src="images/AD-3.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<b>- Step 5:</b>
In the Administration window, Leave everything default. Click on Next.
<p>
<img src="images/AD-4.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<b>- Step 6:</b>
In the Security Settings windows, Leave everything as default.
<p>
<img src="images/AD-5.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<b>- Step 7:</b>
In this section the system will review your configuration to allow you to create.When review is done,then click on Review + create.
<p>
<img src="images/AD-7.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<b>- Step 8:</b>
This image displays the Summary of the settings you made in the previouse step. You should remember them.
<p>
<img src="images/AD-6.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<b>- Step 9:</b>
We can see that, the deployment under progress. (This can take up to 30 to 40 minutes).

<p>
<img src="images/AD-9.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<b>- Step 10:</b>
You can now see, the deployment is completed. 
<p>
<img src="images/ad-final.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h1><u>***The following steps will guide you to create VM.***</u></h1><br />


<b>- Step 1:</b>
 Search for a Virtual Machine in the searchbar above.
<p>
<img src="images/vm-1.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<b>- Step 2:</b>
<p>We have to create a Windows server Virtual Machine for Azure AD DS Management Tools. Follow the below screenshot to create a VM.
<img src="images/vm-2.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<b>- Step 3:</b>
 In the Networking tab, select the Virtual Network and Subnet connected to the Azure AD Domain Services. Then click Review + create.
<img src="images/vm-3.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<b>- Step 4:</b>
 Now, it will validate all the data entered by me and show you the Validation passed. Click on Create.
<img src="images/vm-4.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<b>- Step 5:</b>
<p> Now, it will validate all the data entered by me and show you the Validation passed. Click on Create.
<img src="images/vm-5.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/><br>
<img src="images/vm-6.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>

<b>- Step 6:</b>
 It is time to Add the DNS IP address (Azure AD Domain Services) on the Vnet. From the Searchbar, search for the Virtual Network and click on it. The images below illustrates the process. 
<p><img src="images/vm-7.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/><br>
<img src="images/vm-8.1.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<b>- Step 7:</b>
Below Images shows how you . 
<p><img src="images/vm-9.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/><br>
<img src="images/vm-10.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/><br>
<img src="images/vm-11.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/><br>
<img src="images/vm-12.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="images/vm-12-final.png" alt="Azure active Directory Domain Service"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<b>Conclusion</b>
 This ends our process of creating Azure AD Domain Service.

<b>You can install the following features from the console to make your system run smoothly.</b><br>
*Role Administration Tools<br>
*ADDS and AD LDS Tools<br>
*Active Directory module for Windows PowerShell<br>
*AD DS Tools<br>
*AD DS Snap-ins and Command-Line Tools<br>
*Group Policy Management Console (GPMC)<br>
*DNS Server Manager<br>

</p>

<br />
