In this lab, I will explore the enumeration of systems using Linux and Windows command line tools. We end this lab by actively scanning with tools.

Active Scanning with Tools

1. Boot up Kali Linux server.

2. Type in the following command: "service postgresql start" in the terminal.

<img width="244" height="25" alt="image" src="https://github.com/user-attachments/assets/c68cc824-0714-4c81-b9be-4dd7adc520dd" />

Result of Step 2

3. Type in the following command: "cd armitage" in the terminal.

<img width="187" height="25" alt="image" src="https://github.com/user-attachments/assets/5f193a1d-007e-41d8-9605-eee6baf5aaad" />

Result of Step 3

4. Type in the following command: "msfconsole" in the terminal. This will start Metasploit.

<img width="459" height="274" alt="image" src="https://github.com/user-attachments/assets/82a2ddb8-9632-4fe5-a881-602862c7fb54" />

Result of Step 4

5. Type in the following command: "db_nmap -T4 -A -v 192.168.1.*" in the msfconsole. To scan hosts. This step will take up to 5 minutes to complete.

<img width="464" height="164" alt="image" src="https://github.com/user-attachments/assets/3d806a9a-1511-41c1-9ddc-42a2059406f6" />

Result of Step 5

6. Type in the following command: "hosts" in the msfconsole. To view all of the discovered hosts.

<img width="463" height="214" alt="image" src="https://github.com/user-attachments/assets/ba8994c3-39c6-436e-9067-ad099791f56a" />

Result of Step 6

7. Type in the following command: "./armitage" in the msfconsole. To start Armitage. Click connect and then click Yes.

<img width="467" height="325" alt="image" src="https://github.com/user-attachments/assets/95d7ff10-5a87-4234-bdb8-9f17ae8254c9" />

Result of Step 7

8. Wait for the process to go through.

<img width="256" height="107" alt="image" src="https://github.com/user-attachments/assets/1b4b68d7-5547-447d-91b8-8e997509b7f3" />

Result of Step 8

9. Righ click on the layout and Select Auto-Layout and then click Stack.

<img width="474" height="218" alt="image" src="https://github.com/user-attachments/assets/a3bb8166-6319-424d-8e01-b39ef3d62920" />

Result of Step 9

10. Right click on the printer IP Address and press Scan.

<img width="127" height="102" alt="image" src="https://github.com/user-attachments/assets/018385e1-53b5-4755-af8b-8b2d79a63554" />

Result of Step 10

11. Scan Results

<img width="473" height="174" alt="image" src="https://github.com/user-attachments/assets/deeb8591-89cc-4fc7-9696-fea41d233e8d" />
