
<h1>Troubleshoot User Login</h1>
This tutorial shows and resolves common user log-in issues. 

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10 (21H2) **Client-1**
- Windows (Windows Server 2022 Datacenter Azure Edition) **DC-1**

<h2>High-Level Steps</h2>

**User Account Expired**
- Step 1: Attempt to Remote log into Client-1 account. 
- Step 2: Remote log-in to DC-1 as admin (mydomain.com\jane_doe) and allow 2 months of domain access to Client-1.
- Step 3: Attempt to Remote log-in to Client-1 account.


<h2>Actions and Observations</h2>

Step1: Attempt to Remote log-in to Client-1 account (mydomain.com\bab.cop). Observe the disclaimer
<p>
  
![image](https://github.com/user-attachments/assets/62d1e802-305a-4683-b9de-391d98d1631c)
</p>

![image](https://github.com/user-attachments/assets/3ab6ffdb-5617-424a-8917-9180bb5293c6)

<br />

<p>
Step 2: Log-in to DC-1 account as Admin (mydomain.com\jane_doe). Select the Windows icon. Select 'Windows Admin. tools' then select 'Active Directory User and Computers'. 
Select the domain name and select the OU: _EMPLOYEES. Find and double-click on the 'bab.cop' file. 
  
![image](https://github.com/user-attachments/assets/67161044-ef98-497e-88e7-e38efd61fdc9)
</p>

In the 'Account' tab. Go to the 'Account expires' and allow an additional 2 months of access. Select 'Apply' and 'Ok'. 

![image](https://github.com/user-attachments/assets/64174fc8-fd36-4c9f-9fe5-cfeb8a024aa3)

<p>

<br />

<p>
Step 3: Remote log-in to Client-1 as 'mydomain.com\bab.cop'.
  
![image](https://github.com/user-attachments/assets/309a2a08-ee12-4862-9c61-8ddda3e5b47a)

![image](https://github.com/user-attachments/assets/9a1a6c78-7906-4b64-9d34-573619f11610)

<br />
