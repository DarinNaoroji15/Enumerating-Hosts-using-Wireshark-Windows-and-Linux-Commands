# Enumerating Hosts using Wireshark Windows and Linux Commands

In this lab, I will explore the enumeration of systems using Linux and Windows command line tools. We will start by passively scanning.

Passive Scanning

1. Start up your Kali Linux Server.

2. Once signed in, click on the Linux terminal icon.

<img width="470" height="331" alt="image" src="https://github.com/user-attachments/assets/6a11d32e-c1fa-4e2a-a8a8-98b1e5e5dff6" />

Result of Step 2

3. Type in the following command: "ifconfig" into the terminal. This command will reveal the IP Address of the system.

<img width="469" height="269" alt="image" src="https://github.com/user-attachments/assets/51a78abe-70ff-4189-a762-3bdbe0a3d8a4" />

Result of Step 3

4. Type in the following command: "ifconfig > ip1.txt" into the terminal. This command will save our IP Address configuration.

<img width="208" height="34" alt="image" src="https://github.com/user-attachments/assets/d1460ae3-78ac-45a8-b77d-5948487b7b93" />

Result of Step 4

5. Type in the following command: "cat ip1.txt" into the terminal. This will allow you to view the IP Address configuration in this file.

<img width="461" height="226" alt="image" src="https://github.com/user-attachments/assets/f40a6a2c-1a4c-48ac-871c-c10a3685aa82" />

Result of Step 5

6. Type in the following command: "cat ip2.txt" into the terminal. This will allow you to view the IP Address configuration in this file.

<img width="461" height="233" alt="image" src="https://github.com/user-attachments/assets/1d2b7e35-4b67-4e76-92e0-14b3a9240aea" />

Result of Step 6

7. Type in the following command: "ifconfig eth0 0.0.0.0 up" into the terminal. Our system now will not have an IP Address.

<img width="251" height="28" alt="image" src="https://github.com/user-attachments/assets/d2157adf-1e80-4608-814c-af12140acf4e" />

Result of Step 7

8. Type in the following command: "ifconfig" into the terminal. To verify we no longer have an IPv4 address listed for eth0.

<img width="437" height="214" alt="image" src="https://github.com/user-attachments/assets/ee69595b-1f8d-4da8-9cc2-48b06018c8eb" />

Result of Step 8

9. Type in the following command: "wireshark" into the terminal. This will open Wireshark. There will be an error, select OK to the error when Wireshark opens.

<img width="462" height="334" alt="image" src="https://github.com/user-attachments/assets/41f0dab1-42e0-46c7-971c-f3aaeb0e36eb" />

Result of Step 9

10. Once Wireshark is booted up, click on Capture from the top ribbon. Then choose Interfaces.

<img width="475" height="413" alt="image" src="https://github.com/user-attachments/assets/e56fbc38-4f44-4fd8-a8bf-8a30d1708c22" />

Result of Step 10

11. Then check off the eth0 box and click start.

<img width="267" height="88" alt="image" src="https://github.com/user-attachments/assets/694f4863-ca96-4162-b91c-174cfe7f27ab" />

Result of Step 11

12. Packets will start to appear in the list and run.

<img width="469" height="391" alt="image" src="https://github.com/user-attachments/assets/5ae58424-bfa6-4955-8273-795aa73aeb7f" />

Result of Step 12

13. To stop the Wireshark capture, click on the red button at the top ribbon.

<img width="476" height="90" alt="image" src="https://github.com/user-attachments/assets/e3d12090-0360-4ec5-b7a7-14a6ac923638" />

Result of Step 13

14. Click "Quit" to escape the Wireshark. It will ask if you'd like to quit without saving. Click on that option.

<img width="473" height="319" alt="image" src="https://github.com/user-attachments/assets/48dab94a-80a2-41bd-a0c5-aa2a7ae6e0b0" />

Result of Step 14

15. Type in the following command: "ifconfig" into the terminal. To check on the IP Address of the system.

<img width="425" height="224" alt="image" src="https://github.com/user-attachments/assets/a34b42e3-59a7-47d8-9871-f5a933a0bbb3" />

Result of Step 15

16. Type in the following command: "ifconfig eth0 192.168.1.101 netmask 255.255.255.0" into the terminal. To set up IP Address and Subnet Mask.

<img width="403" height="23" alt="image" src="https://github.com/user-attachments/assets/51de8eaf-d103-4a6c-bf65-eeb885ea476a" />

Result of Step 16

17. Type in the following command: "route add default gw 192.168.1.254" into the terminal. To set the gateway up.

<img width="312" height="26" alt="image" src="https://github.com/user-attachments/assets/ee5d14c0-2d56-45ee-83fa-faf258b8a78c" />

Result of Step 17

18. Type in the following command: "cp /etc/resolv.conf  /etc/resolv.conf.backup1" into the terminal. This will backup the current resolv.conf file.

<img width="370" height="23" alt="image" src="https://github.com/user-attachments/assets/1b790cbb-9e5a-461a-bfde-c8ff3e2a484b" />

Result of Step 18

19. Type in the following command: "root@kali2:~# cat etc/resolv.conf.backup1" into the terminal. This will allow you to view this IP Address configuration file.

<img width="278" height="50" alt="image" src="https://github.com/user-attachments/assets/bb72f05c-ae4b-4edd-af71-52fdab86496e" />

Result of Step 19

20. Type in the following command "echo nameserver 192.168.1.10 > /etc/resolv.conf" into the terminal. This is to set the DNS server up.

<img width="404" height="26" alt="image" src="https://github.com/user-attachments/assets/383f1b48-18e8-4e32-8428-b5cac709d4c9" />

Result of Step 20

21. Type in the following command: "cat /etc/resolv.conf" into the terminal. To view the contents of this file.

<img width="235" height="40" alt="image" src="https://github.com/user-attachments/assets/6ca9678a-e7a2-4e48-b670-f6b78f313f51" />

Result of Step 21

22. Type in the following command: "ifconfig" into the terminal. To verify the correct IPv4 address is listed eth0.

<img width="459" height="227" alt="image" src="https://github.com/user-attachments/assets/b3734ec5-f6bf-4d0b-8625-fba47975dd4e" />

Result of Step 22
