### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
 
## Aim: 
To  configure the Network server and end device for transferring data on the network
## Components required: 
End node stm 32 development kit , Dragino LPS8, Network server 

## Theory :
When working with sensitive applications or files, saving progress on your local device is a start, but what if you lose access to your device? Network servers address this problem by hosting the files and programs most pertinent to the network and enabling access for consistent, real-time use. 

As a result, personnel or network clients can instantly access important data or tools while also facilitating collaboration between users. Multiple users can make changes to the same program or document for continued development over the course of a project. Via a secure login, remote users can connect to the home network.
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/59db9b76-ddd5-4d6a-9075-8db233f5e479)


In the above graphic, the circle represents an organization network where a network server facilitates collaboration and file sharing between network clients (devices).

 The role of a network server, then, is to provide users with a set of services and access to resources on the network. These features include:

Permissioned access and log-ins for network users Gateway access to the Internet for an organization Centralized location for network resources  Shared access to devices on the network like a printer or a scanner Hosts multi-user apps like email servers, web applications, or CRM

## Procedure :

 1. login to the network server using login link  https://iot.saveetha.in/
 2. Click on the nework server as shown blow
    
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1bd434ca-1426-4102-8384-94473483543e)
 3. Click on the add gateway 
 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/47c2e08d-6598-4437-8b07-f213d6f3b8ac)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/e62ff028-99bc-485e-9808-fbb6e124f8b2)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/a2e3ae58-6402-49e8-8f96-679059c1842c)
4. Click on the lora options , lora - frequency plan 

5. Click on channels and create a new channel after which you can add a new end device
   
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1fb72be5-e48d-4cde-a329-0cfb0d29070f)

6. Add the attributes in the end device as  shown below 

 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/00bff30b-42fc-42d5-9540-285d270e41cb)
 
7.Using AT commands configure end device in serial port utility
AT Commands to set initially (Mandatory)
 AT+FDR // To do factory data reset
 AT+NJM=1 // To set OTAA mode
 AT+ADR=1 // To enable the ADR
 AT+TDC=600000 // To set the default sampling interval as 10 minutes
(Should not give below 5 minutes)
 AT+CLASS=C // To set class C
 AT+DEUI=XX XX XX XX XX XX XX XX // To set Device EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX // To set APP EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX //
To set APP Key
 ATZ // To take effective action on below settings (As like saving)



## OUTPUT 

<img width="1919" height="1065" alt="image" src="https://github.com/user-attachments/assets/b87b05de-5d92-4b85-a776-ec5935fc63e8" />

<img width="1920" height="1200" alt="Screenshot (115)" src="https://github.com/user-attachments/assets/e2a8ca0b-7a29-4edb-9871-2c7e740616d1" />

<img width="1920" height="1200" alt="Screenshot (116)" src="https://github.com/user-attachments/assets/5d65b5da-d5d7-41f3-8ca0-671f473b9535" />

<img width="1920" height="1200" alt="Screenshot (117)" src="https://github.com/user-attachments/assets/3ac981e9-e6ad-4fdf-9439-26808ba46994" />

<img width="1920" height="1200" alt="Screenshot (118)" src="https://github.com/user-attachments/assets/4584860a-b9fe-40f1-af44-4bd7ed5d58c3" />

<img width="1920" height="1200" alt="Screenshot (119)" src="https://github.com/user-attachments/assets/4ab75688-7d47-4d15-82ca-1fc36df2d789" />

<img width="1920" height="1200" alt="Screenshot (120)" src="https://github.com/user-attachments/assets/73a4a54c-b110-4ca8-b2b4-450d25bb7572" />

<img width="1920" height="1200" alt="Screenshot (121)" src="https://github.com/user-attachments/assets/3dfdf80f-ac7f-41b5-92ee-6522dc674d94" />

<img width="1920" height="1200" alt="Screenshot (122)" src="https://github.com/user-attachments/assets/f4643b91-4585-4a65-afcb-dfced159b736" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/04faceae-5ee7-4d42-aa83-66c61e56a3b4" />

<img width="1812" height="1127" alt="1" src="https://github.com/user-attachments/assets/cfeb6696-0965-4132-b204-97c51113183d" />
<img width="1812" height="1127" alt="1" src="https://github.com/user-attachments/assets/22b01140-46d0-4200-a26e-09a07e71ac58" />
<img width="1785" height="1127" alt="3" src="https://github.com/user-attachments/assets/43165fac-58a5-4706-9b7a-f0f7e8bed93f" />
<img width="1777" height="1132" alt="4" src="https://github.com/user-attachments/assets/eb5ea4d3-c530-4a58-90ef-1c1b5bb3922d" />
<img width="1796" height="1124" alt="5" src="https://github.com/user-attachments/assets/8e1c39a8-67f8-4ac7-9d98-bbdb9003997b" />
<img width="1796" height="1124" alt="5" src="https://github.com/user-attachments/assets/1c0d88b0-cced-4f50-bc07-0870732c4495" />
<img width="1793" height="1111" alt="7" src="https://github.com/user-attachments/assets/9e386477-b8a8-45f5-bc65-659881f53636" />
<img width="1806" height="1109" alt="8" src="https://github.com/user-attachments/assets/2006acb1-5587-48d5-a87b-bd5cbea7ded3" />
<img width="1781" height="1104" alt="9" src="https://github.com/user-attachments/assets/6e73371e-4a26-4dae-9812-34968da755f3" />
<img width="1827" height="1150" alt="11" src="https://github.com/user-attachments/assets/08bd7a79-c9cb-45bb-977c-a9fbdb5b194e" />
<img width="1804" height="1104" alt="13" src="https://github.com/user-attachments/assets/4871affb-c87b-4b4c-8ed9-f8939d782d32" />
<img width="1812" height="1131" alt="14" src="https://github.com/user-attachments/assets/6f444141-f901-42bd-af73-f094e28c0957" />
<img width="1789" height="1107" alt="15" src="https://github.com/user-attachments/assets/577d6a9c-0557-4f23-8ed8-8274c07bef06" />
<img width="1805" height="1136" alt="111" src="https://github.com/user-attachments/assets/4d58afe7-1949-4814-8828-65937944aaf4" />
<img width="1829" height="1087" alt="132" src="https://github.com/user-attachments/assets/d8b694be-f311-44f0-b1bd-6c1de31bd2f2" />



## Result: 

  The Network server and end device for transferring data on the network has been accomplished.
