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

<img width="1680" height="1060" alt="1" src="https://github.com/user-attachments/assets/1871354d-ceca-4e02-93a7-662fd7df2622" />
<img width="1729" height="1069" alt="2(1)" src="https://github.com/user-attachments/assets/96bcc017-0c1b-4c4e-9948-37d27766b74e" />
<img width="1625" height="1107" alt="3" src="https://github.com/user-attachments/assets/09c38f59-992a-433a-9a0b-5ccdda55b567" />
<img width="1920" height="1200" alt="4" src="https://github.com/user-attachments/assets/a7b99e0e-2a4b-47c3-96f6-b57e9fe4c691" />
<img width="1920" height="1200" alt="5" src="https://github.com/user-attachments/assets/c16983ce-215f-41f6-8e20-b11e628fa209" />
<img width="1920" height="1200" alt="6" src="https://github.com/user-attachments/assets/76c6b6eb-9ec7-4b8f-8bda-cdd4626d7559" />
<img width="1729" height="1081" alt="7(1)" src="https://github.com/user-attachments/assets/14589a0f-0840-4e15-9eff-3e262c2f1db9" />
<img width="1729" height="1081" alt="8(1)" src="https://github.com/user-attachments/assets/ef3e310f-a7a4-471a-9436-d03222070433" />
<img width="1729" height="1081" alt="9(1)" src="https://github.com/user-attachments/assets/bcbdbfbc-5f1f-4aab-9f66-6bf3965610b5" />


## Result: 

  The Network server and end device for transferring data on the network has been accomplished.
