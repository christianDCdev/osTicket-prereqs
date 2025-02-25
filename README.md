<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Prerequisites</h2>

- Create a virtual machine in Azure
- Download <a href="https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD">osTicket Installation Files</a> within the virtual machine
- Enable IIS in Windows with CGI
- Install PHP manager for IIS from the <a href="https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD">osTicket Installation Files</a>
- Install the Rewrite Module from the <a href="https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD">osTicket Installation Files</a>
- Install VC_redistx86 from the <a href="https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD">osTicket Installation Files</a>
- Install MYSQL 5.5.62 from the <a href="https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD">osTicket Installation Files</a>
- Install HeidiSQL from the <a href="https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD">osTicket Installation Files</a>

<h2>Installation Steps</h2>
<h3>&#9332; Create a Virtual Machine(VM) in Azure</h3>

<p>

- Create a resource group in Azure
- Create a virtual machine
    - Under "Image", select Windows 10 Pro version 22H2
    - Under "Size", select option with at least 2 vcpus
    - Under "Select Inbound Ports", confirm RDP(3389) is selected
    - Review and create
</p>
<br />

<h3>&#9333; Connect to your VM through Microsoft Remote Desktop App</h3>

<p>

- Find your VM's public IP address and copy it
- Open Microsoft Remote Desktop App
- Paste VM's public IP address into "Computer" field then connect to VM
<img src="https://i.imgur.com/Z2iVbds.png" height="80%" width="80%" alt="Remote desktop IP"/>
  
</p>
<br />

<h3>&#9334; Download <a href="https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD">osTicket Installation Files</a> within the virtual machine </h3>

<p>

- Copy <a href="https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD">osTicket Installation Files</a> link
- Within the VM, open a browser, paste link into search bar, then download the files
  
</p>
<br />

<h3>&#9335; Enable IIS</h3>

<p>

- Open the control panel and select "Programs"
- Click on "Turn Windows features on or off"
- Scroll down to and expand "Internet Information Services(IIS)"
- Expand "World Wide Web Services"
- Expand "Application Development Features"
- Enable CGI then hit "Ok"
  
</p>
<br />

<h3>&#9336; Install PHP Manager</h3>

<p>

- Install "PHPManagerForIIS_V1.5.0.msi" from <a href="https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD">osTicket Installation Files</a>
  
</p>
<br />

<h3>&#9337; Install Rewrite Module</h3>

<p>

- Install "rewrite_amd64_en-US.msi" from <a href="https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD">osTicket Installation Files</a>
  
</p>
<br />

<h3>&#9338; Create a New Directory</h3>

<p>

- Open File Explorer
- Navigate to Windows (C:) Drive
- In the Windows (C:) Drive, create a new folder titled "PHP"
  
</p>
<br />

<h3>&#9339; Extract "php-7.3.8-nts-Win32-VC15-x86.zip" </h3>

<p>

- Extract "php-7.3.8-nts-Win32-VC15-x86.zip" files into newly created "PHP" folder in Windows (C:) Drive
  
</p>
<br />

<h3>&#9340; Install "VC_redist.x86.exe"</h3>

<p>

- Install "VC_redist.x86.exe" from <a href="https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD">osTicket Installation Files</a>
  
</p>
