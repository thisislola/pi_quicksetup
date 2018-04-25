# pi_quicksetup

### In config.txt, add at the end:
dtoverlay=dwc2

### In cmd.line, add this between 'rootwait' and 'quiet'
modules-load=dwc2,g_ether

### Create an empty file called "ssh" without any type file
### no .txt nor anything, choose '* all files'

### Config steps on machine: 
	1. Plug the Raspberry Pi Zero from the DATA plug (second micro USB) to the machine. You can use a regular USB phone charging cable.
	2. Let it boot up for about 1 minute
	3. On Windows, right click on your Internet connection and open Network and Sharing Center and then Change Adapter Options
	(Control Panel\Network and Internet\Network and Sharing Center)
	4. Find your Ethernet connection and locate the Pi's (called something like Ethernet/RSD)
	5. Right click on your main Ethernet Network icon, click on Properties and then Sharing. Enable it and find the Pi's ethernet connection. Ok, ok, to all and TADA! 

### SSH to your pi using raspberrypi.local on port 22:
	** Username: pi
	** Password: raspberrypi 
	// Change the password using the command 'sudo passwd' without the quotes

Now you have a plug-ssh and play linux terminal with internet connection! 
