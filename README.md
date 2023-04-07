# Setup a Ubiquiti-NanoBeam-Setup
NanoBeam "Point to Point" Walkthrough | Ubiquiti
<h2>Description</h2>
Our company uses Ubiquiti products for many different jobs. We like to use NanoBeams as a wireless bridge that can go as far as 9.3 miles with proper line of sight. Using these "point to point" devices we are able to allow security systems to communicate between cameras without the need for any wires. 
<br />

<h2>Program walk-through:</h2>

<p align="center">
<br/>
•	Before starting this guide you can reference this link for Ubiquiti's setup guide. 
<br/>
https://dl.ubnt.com/qsg/NBE-5AC-Gen2/NBE-5AC-Gen2_EN.html
<br/>
<img src="https://i.imgur.com/blxuTOv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
<br/>
•	Today we will be setting up 14 different NanoBeams.
<br/>
<img src="https://i.imgur.com/3DCxWIA.jpg" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
<br/>
•Unbox your device. You should see these items inside <br/>
<img src="https://i.imgur.com/09iegOK.png" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
<img src="https://i.imgur.com/kd94gTH.jpg" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
•	The Nanobeam has to have 24V POE. We need to use the block it comes with. Using ethernet cables, plug the POE port from the 24V block into the main port on Nanobeam and the LAN port on block into your switch.
<br/>
<img src="https://i.imgur.com/5bOTZlk.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
•	You need to hop on your Unifi portal and see what clients are connected to your network. Find the MAC address of the Nanobeam on your client list to find it's IP address. The default for Nanobeam is 192.168.1.20 <br/>
<img src="https://i.imgur.com/8wM4rz5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
•	Now we need to change the IP of our computer to match that range. Go to Settings -> Network and Internet -> Ethernet -> Change Adapter Options <br/>
•Double click the Ethernet Adapter, Click properties, Double click Internet Protocol Version 4, change your IP range to match the address given by the point-to-point device (DON’T FORGET TO CHANGE YOUR IP BACK TO AUTOMATIC WHEN DONE) 
<br/>
<br/>
<img src="https://i.imgur.com/2Hm1tgl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
•	Once this step is done you can put IP into browser and the nanobeam portal should show up <br/>
<img src="https://i.imgur.com/0Zl0BJU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
<br/>
• Setup the device settings <br/>
<img src="https://i.imgur.com/91TQQ7f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<img src="https://i.imgur.com/TXEsCYk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/
<br/>
<br/>
<br/>
•	While in portal go to SYSTEM and name the device. <br/>
<img src="https://i.imgur.com/Uotb8Zp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<br/>
•	As soon as you know what the device name is, label the phsycial Nanobeam. This will make installation and troubleshooting easy for the techs and future network admins <br/>
<img src="https://i.imgur.com/OYbsUFj.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<img src="https://i.imgur.com/ESX9IPa.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<br/>
•	Then go to wireless, the first nanobeam needs to be tabbed as an Access Point and will be the uplink to the internet from the office or wherever the router is located.
<br/>
<img src="https://i.imgur.com/gtKHt7V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
•	The final step before leaving the browser is to assign the device to DHCP. This will automatically assign an available IP address on the network, removing the default address. This also prevents issues when we plug in our new Nanobeam so there isn't multiple devices with the same address. <br/>
<img src="https://i.imgur.com/TtqEUZY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<br/>
<br/>
•	You will now have your domain show under your domain list, click it. <br/>
•	Click on Users, it you should now be here 
<br/>
<img src="https://i.imgur.com/zNawfAn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<br/>
•Leave the access point plugged into the switch and plug your next Nanobeam into a new port the same way as the first.<br/>
•Go to SSID once normal changes are made (DO NOT select access point), find the first point to point that was marked as Access Point, then LOCK TO AP. Apply changes.
•Before changing the second AP to DHCP go to Dashboard and wait to see if the 2 devices have connected to eachother .
<br/>
<img src="https://i.imgur.com/33xfe2J.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<br/>
•Once you have verified they are able to connect we can rinse and repeat with all the other pairs.
<br/>
•	All we have to do now is store the Nanobeams back in their boxes, writing the same name from the corresponding label onto the box. This makes life easier for whoever is installing these on site.
<br/>
<img src="https://i.imgur.com/yDqpIa0.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
<br/>
• We have successfully created our point to points for installation! 
