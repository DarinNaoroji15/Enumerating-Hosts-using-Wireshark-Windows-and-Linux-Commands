# Enumerating Hosts using Wireshark, Windows, and Linux Commands

In this lab, I will explore the enumeration of systems using Linux and Windows command line tools. This section we will start by actively scanning with commands.

Active Scanning with Commands

1. Boot up your Windows 10 Server.

2. Begin with right-clicking on the Windows Desktop key and sign out.

<img width="259" height="233" alt="image" src="https://github.com/user-attachments/assets/f899f594-d883-43ba-9f9b-72df425c2d2d" />

Result of Step 2

3. We will switching over to the Admin account in the Login interface.

4. Right click on the command prompt icon on the desktop and select Run as administrator.

<img width="192" height="263" alt="image" src="https://github.com/user-attachments/assets/a1f2673e-c756-4b16-a560-57d8b3160a33" />

Result of Step 4

5. Type in the following command: "net view" in the cmd prompt. This command will attempt to enumerate machines.

<img width="467" height="188" alt="image" src="https://github.com/user-attachments/assets/f98af32e-1661-4c09-a8a7-623839106a0b" />

Result of Step 5

6. Type in the following command: "net view /domain" in the cmd prompt. This command will attempt to enumerate all the domains.

<img width="337" height="128" alt="image" src="https://github.com/user-attachments/assets/faff95e7-b353-482e-83e8-7ac5f9452986" />

Result of Step 6

7. Type in the following command: "net view /domain:campus" in the cmd prompt. To attempt again to enumerate all the domains.

<img width="361" height="130" alt="image" src="https://github.com/user-attachments/assets/e305a5d3-7609-4ad6-be65-2a32bc2490c1" />

Result of Step 7

8. Type in the following command: "net view /domain:workgroup" in the cmd prompt. To attempt as well to enumerate all of the domains.

<img width="462" height="154" alt="image" src="https://github.com/user-attachments/assets/f00035e7-eab1-490a-9f2b-e26ddcbf88d9" />

Result of Step 8

9. Type in the following command: "net view \\server" in the cmd prompt. To attempt to enumerate the shares on the machines named server.

<img width="400" height="198" alt="image" src="https://github.com/user-attachments/assets/d3c5e99e-1d4c-435f-8c4e-47176375739f" />

Result of Step 9

10. Type in the following command: "net view \\metasploitable" in the cmd prompt. To attempt to enumerate the shares on the machines named metasploitable.

<img width="392" height="197" alt="image" src="https://github.com/user-attachments/assets/ae222d4f-bd81-4671-94a6-66df4ca82cb5" />

Result of Step 10

11. Type in the following command: "nbtstat -a server" in the cmd prompt. To attempt to enumerate the IP and MAC Address of the machine named server.

<img width="416" height="277" alt="image" src="https://github.com/user-attachments/assets/39b5579a-2ccb-40e1-b48f-b8e77a5a218c" />

Result of Step 11

12. Type in the following command: "nbtstat -a METASPLOITABLE" in the cmd prompt. To attempt to enumerate the IP and MAC Address of the machnie named metasploitable.

<img width="427" height="260" alt="image" src="https://github.com/user-attachments/assets/e7e75e02-abef-4a62-b191-d97df944ea17" />

Result of Step 12
