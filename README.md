# Active Directory Lab
Skills Learned: Active Directory, Powershell, Windows Server, Windows Networking, Virutalization
<h2>Description</h2>
I am following a tutorial video found <a href="https://www.youtube.com/watch?v=MHsI8hJmggI&t=0s">here</a>. <br/> <br/>
I created an Active Directory home lab environment using Oracle Virtual Box. I created 2 virtual machines, one running Windows Server 2019 and the other a Windows 10 client. The Server 2019 VM acted as the Domain Controller and had Active Directory Domain Services, RAS, NAT, and DHCP services installed on it. It has 2 network adapters, one connected to my home network and one connected to an internal network. I assigned the internal network adapter an IP address, renamed the server, and after installing and configuring Active Directory, I created a Domain Admin account that I used to install RAS and NAT so the client can connect to the internet and DHCP so the client will automatically be assined an IP address. Once the VM was set up I used a Powershell script to automate the creation of over 1,000 users in Active Directory. I then set up the Windows 10 VM, changing the network adapter to the internal network, checked for the IP address and internet connectivity provided by the domain controller, added it to the domain, and logged into it with one of the user credentials created from the Powershell script. This concluded the setup of the lab environment. 

<br/>

<h2>Configruring Internal Network Adapter on Domain Controller</h2>

<p align="center">
<img width="737" alt="add internal IP" src="https://user-images.githubusercontent.com/67126494/190018574-c3171907-2e95-4a0f-8014-f4cad26e5f7c.png">
</p>

<br/>

<h2>Server Manager showing installed services: Active Directory Domain Services, Remote Access with NAT, and DHCP </h2>

<p align="center">
<img width="635" alt="installed services" src="https://user-images.githubusercontent.com/67126494/190018810-68109bc1-b975-47cf-b052-303c380e9a7f.png">
</p>

<br/>

<h2>Powershell Script Running, Creating users in Active Directory </h2>

<p align="center">
<img width="487" alt="Script running" src="https://user-images.githubusercontent.com/67126494/190019082-22d99212-e2ed-4046-bc42-07e04fd70172.png">
</p>

<br/>

<h2>Windows 10 Client ipconfig showing DHCP assigned IP address and Internet connectivity through Routing and NAT </h2>

<p align="center">
<img width="384" alt="client assigned IP" src="https://user-images.githubusercontent.com/67126494/190019303-b5d4ca6c-89f3-48be-9c78-ecd4de709ab6.png">
</p>

<br/>

<h2> DHCP showing Windows 10 Client in Leases</h2>

<p align="center">
<img width="402" alt="address leases" src="https://user-images.githubusercontent.com/67126494/190019430-5e2ab6ad-cad8-40da-af01-a330f8417d48.png">
</p>

<br/>

<h2> Active Directory showing Windows 10 Client added in Computers List</h2>

<p align="center">
<img width="340" alt="client in computer list" src="https://user-images.githubusercontent.com/67126494/190019500-168db6b7-9873-4162-8e17-7417ba6e5ca5.png">
</p>

<br/>

