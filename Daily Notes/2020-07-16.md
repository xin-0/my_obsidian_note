Connect two linux by ether cable:

1. Connect two with cable
	On PC 1:
	1. `$ ifconfig` to get Hardware address/MAC
		- de.g. `HWaddr 00:e0:4c:4c:a6:8e`
	2. In 'edit connection' --> 'add' --> 'ether'
		- fill device with `HWaddr`
	3. Go to tab 'IPv4'
		- chooes manual 
		- set ip: 192.168.80.xx(PC1)
	On PC 2:
	repeat 1-3 as on PC1, set ip in the form 192.168.80.xx(PC2) but different.
	
Connect PC2 from PC1 using:
`ssh usr@192.168.80.xx(PC2)`