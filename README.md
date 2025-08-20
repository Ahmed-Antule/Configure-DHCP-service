# Configure-DHCP-service

Dynamic Host Configuration Protocol (DHCP) – Automated IP Address Management DHCP (Dynamic Host Configuration Protocol) is a network management protocol that automatically assigns IP addresses, subnet masks, default gateways, and DNS settings to devices on a network. This eliminates the need for manual IP configuration, ensuring efficient and conflict-free network management.

Key Benefits:

✅ Automated IP Assignment – Reduces manual configuration and errors.

✅ Efficient IP Management – Dynamically allocates and reclaims unused IP addresses.

✅ Scalability – Ideal for networks with a large number of devices.

✅ Centralized Control – Simplifies administration with a dedicated DHCP server.

Summary
In this project, I installed and configured the DHCP protocol on Windows Server. I created an IP address pool, allowing the DHCP server to automatically assign IP addresses to client machines, ensuring efficient and dynamic network management.

### Step - 1 <br>
i. Open Server Manager, then navigate to "Add Roles and Features.
<img width="1366" height="706" alt="Capture1" src="https://github.com/user-attachments/assets/1d1aea31-18cd-43cf-b5f5-2b8fa2451e6c" />

ii. In "Server Roles," select and add the DHCP Server role.
<img width="830" height="586" alt="Capture2" src="https://github.com/user-attachments/assets/907faa61-f73b-4da7-a87e-5c0ccf25e450" />

iii. In the "Confirmation" section, click "Install" to set up the DHCP Server.
<img width="807" height="578" alt="Capture3" src="https://github.com/user-attachments/assets/f297027e-5645-4c7e-a21a-1973de378ad1" />

iv. Once the installation is complete, click on "Complete DHCP Configuration" and follow the steps as shown in the screenshots.
<img width="810" height="571" alt="Capture4" src="https://github.com/user-attachments/assets/188ec7a0-6d49-47df-baed-a2f9cefd1c3e" />
<img width="779" height="572" alt="Capture5" src="https://github.com/user-attachments/assets/2b16a12c-3af5-481c-b7d0-2307d43b6283" />

### Step - 2
i. Go to "Tools" in Server Manager and select "DHCP."
<img width="1366" height="242" alt="Capture6" src="https://github.com/user-attachments/assets/f1acb025-086d-4448-a98a-82b521bf2b19" />
<img width="884" height="708" alt="8" src="https://github.com/user-attachments/assets/97049d96-a3e1-49c9-bf2f-0fe60bbffd96" />

ii. To add an IPv4 scope, right-click on "IPv4" and select "New Scope."
<img width="722" height="746" alt="9" src="https://github.com/user-attachments/assets/f0f0be2a-7c98-41f3-98e1-f5c7af5ac292" />

iii. Enter a name of your choice for the scope and click "Next."
<img width="534" height="434" alt="Capture6 1" src="https://github.com/user-attachments/assets/e1f604cf-c325-4121-9dfa-bea9cc89fd16" />

iv. Specify the Start and End IP range for the scope and click "Next."
<img width="586" height="484" alt="Capture7" src="https://github.com/user-attachments/assets/772593f7-1c17-4600-a73e-99b0977918fb" />

v. In "Add Exclusion and Delay," skip assigning any excluded IPs and proceed by clicking "Next."
<img width="535" height="448" alt="Capture8" src="https://github.com/user-attachments/assets/701090f3-fe0c-4554-b3ae-4490144a07c0" />
<img width="553" height="444" alt="Capture9" src="https://github.com/user-attachments/assets/a5cddd02-0bf5-4403-b286-10984ac74c0a" />

vii. Enter the Default Gateway IP address and click "Next."
<img width="539" height="447" alt="Capture10" src="https://github.com/user-attachments/assets/5f0dadad-7e57-4327-8da1-6ff070488ed1" />

viii. Click "Next" through the remaining steps until you reach "Finish."
<img width="532" height="439" alt="Capture11" src="https://github.com/user-attachments/assets/31bbdbce-d707-495e-ae97-62804d7eaca4" />

### Step - 3
i. Now lets assign the DHCP IP address to our machine , for this type this command

<img width="419" height="235" alt="Capture12" src="https://github.com/user-attachments/assets/7eb7aae0-8552-42f1-9870-bde264cd670a" />

ii. Go to "Network Properties," select your network adapter, then click on "Internet Protocol Version 4 (TCP/IPv4)."
<img width="382" height="460" alt="Capture13" src="https://github.com/user-attachments/assets/f95e67fe-4d30-4c79-ae80-8b86b37c3dbe" />
<img width="387" height="483" alt="Capture14" src="https://github.com/user-attachments/assets/4e5ca124-42df-4864-85d1-1fc3f5d71723" />

iii. Select "Obtain an IP address automatically" and "Obtain DNS server address automatically," then click "OK."
<img width="428" height="474" alt="Capture15" src="https://github.com/user-attachments/assets/07436a11-96e7-4216-8527-ae63f5cb24fd" />

After this, check the network status—you will see that the IP address has been dynamically assigned by the DHCP server.























