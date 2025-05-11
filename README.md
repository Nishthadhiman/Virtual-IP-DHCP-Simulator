# Virtual-IP-DHCP-Simulator
Virtual IP/DHCP Simulator
Welcome to the Virtual IP/DHCP Simulator! This project allows you to simulate the process of generating an IP block, assigning IP addresses to devices via DHCP, and associating them with different Regional Internet Registries (RIRs). It's a great tool to understand how IP assignment and DHCP work.

Features
IP Block Generator: Generate a random IP block (e.g., 10.0.0.0/24) and assign IP addresses to devices within this block.

Assign IP to Device: Assign an IP address to a device and view all assigned IPs.

Release IP: Release an IP from a device and return it to the pool.

Assign to RIR: Assign a generated IP block to a specific Regional Internet Registry (RIR).

Prerequisites
To use this simulator, you don’t need any special software beyond a web browser. Simply open the HTML file in any browser, and you’re good to go!

How to Use
Generate IP Block: Click on the "Generate IP Block" button to generate a new IP block. This block will look like 10.x.x.0/24.

Assign to RIR: Choose a RIR (e.g., APNIC, ARIN, RIPE NCC, etc.) from the dropdown and click on "Assign Block" to assign your generated IP block to the selected RIR.

Assign IP to Device:

Enter the device name in the input field.

Click "Assign IP" to assign an IP address from the generated block to the device.

A list of all assigned IP addresses will be shown on the page.

Release IP: If you want to release an IP from a device, simply enter the device name and click "Release IP". This will return the IP to the available pool.

File Structure
/index.html               - Main HTML file for the simulator
/README.md                - This README file
Code Overview
IP Block Generation
The IP block is generated randomly with the generateIPBlock() function. It uses the 10.x.x.0/24 format and assigns IPs from 10.x.x.1 to 10.x.x.254.

IP Assignment
The assignIP() function assigns a unique IP address from the available pool to a device. The IP address is removed from the pool once assigned.

IP Release
The releaseIP() function releases an IP back to the pool when a device no longer needs it.

Assigning to RIR
The assignToRIR() function allows users to assign a generated IP block to a specific RIR (Regional Internet Registry). The supported RIRs are:

APNIC (Asia-Pacific)

ARIN (North America)

RIPE NCC (Europe)

LACNIC (Latin America)

AfriNIC (Africa)

Contribution
Feel free to contribute to this project! You can:

Fork the repository

Create a new branch (git checkout -b feature-name)

Make your changes

Submit a pull request
