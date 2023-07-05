# Virtual-Machine-Config
<p align="center">
<img src="https://i.imgur.com/7AUG74j.png" height="40%" width="40%" alt="Microsoft Azure Logo"/>
</p>

<h1>Deploy a Virtual Machine in Azure</h1>
Microsoft Azure is a cloud computing platform with numerous products and services. This guide will demonstrate how to create an account, utilize the portal, and create a virtual machine.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure
- Remote Desktop Connection

<h2>Configuration Steps</h2>

- Step 1: Create Azure Account
- Step 2: Azure portal and resource group
- Step 3: Create a virtual machine
- Step 4: Connect to virtual machine using Remote Desktop Connection

<h3>Step 1: Create Azure Account</h3>
First step is to create an Azure account. You can create an account with $200 of free credit for a month. 

<br>
<br>

<p align="center">
<img src="https://i.imgur.com/8NgUUZu.png" height="80%" width="80%" alt="Azure Free Account"/>
  

Follow all the prompts to create the account. A credit card will be needed but will not be charged until the $200 credit runs out or the account has been active for a month. After you create your account, you are now a tenant in Azure!

<h3>Step 2: Azure portal and resource groups</h3>

The Azure portal is located [here](https://www.portal.azure.com).

In order to utilize some of the services in Azure, a resource group needs to be created. Resource groups will store all resources that you are utilizing in Azure. This example will show how to deploy a Windows 10 virtual machine.

<p align="center">
<img src="https://i.imgur.com/iihvTfI.png" height="80%" width="80%" alt="Azure Resource Groups with circle"/>
</p>

When ready, click create resource groups. From there, you will need to name your resource group and select the region. The region will determine which Azure data center will be utilize. We will name our Lab1. The rousource group will house our VM. Click "Review + Create" once finished.


<h3>Step 3: Create a virtual machine</h3>
<p>
Now we are ready to create our first Virtual Machine!! To do so, click on the virtual machine tab, then click on create.  A few different options will appear, just chose the Azure virtual machine option. From here, we will be presented with quite a few different options. We will only be using the Basics and Networking sections. Be sure that the virtual machine is placed in the resourse group that you just created. Now we will give our VM a name, this will help us differentiate between multiple VM's running simotanously. Im gonna chooose VM1, basic and generic but effective. The region is important, make sure that it's in the same region as the resource group.  Also, when you do pick your os, it may change the region. If this happens, just make sure to change it back.
</p>
<p align="center">
<img src="https://i.imgur.com/0OjIMxR.png" height="80%" width="80%" alt="Virtual Machine Menu with arrow"/>
</p>

<p>
Next, we will have to choose an operating system. Azure offers quite a few different options, you could run one VM with Windows, another with Linux, whatever you'd like! Today we will use Windows 10. Then select a size, keep in mind how much your pc can afford to lend out.  The VMs that we create, once connected, will run off of your computer. Its kind of like having a roomate, who takes up space in your place and uses your resources. Try not to lend out more than half of your max.  If you have 16 gigs of ram(memory), try not to lend out any more than 8, or you could start to compromise preformance.
</p>
<p align="center">
<img src="https://i.imgur.com/dlwDz0k.png" height="80%" width="80%" alt="Create Virtual Machine"/>
</p>

<h3>Step 4: Connect to virtual machine using Remote Desktop Connection (RDP)</h3>


In order to connect to the virtual machine, we will remotely connect to it. To do so, we will use Remote Desktop Connection. You will need the public IP address of the VM. You can find this on the right hand side of the VM menu. You can click copy to clipboard and it copys automaticly.

<p align="center">
<img src="https://i.imgur.com/Muhrj0T.png" height="80%" width="80%" alt="SampleVM menu with arrow and circle"/>
</p>
<br />

<p>
Now go to the search bar and type in remote desktop connection and run. Paste the IP address and enter the user name for the VM that you made earlier. Click connect. If done properly, it will ask for the users password. Click ok and follow all the prompts.
</p>

<p align="center">
<img src="https://i.imgur.com/kXUHRZi.png" height="80%" width="80%" alt="Microsoft Remote Desktop 1"/>
</p>
<br />

<p align="center">
<img src="https://i.imgur.com/tQ5PgyF.png" height="80%" width="80%" alt="Windows 10 VM"/>
</p>

<p align="center">
<img src="https://i.imgur.com/BzkUoGk.png" height="80%" width="80%" alt="Microsoft Remote Desktop"/>
</p>

<p align="center">
<img src="https://i.imgur.com/iAMcQ1M.png" height="80%" width="80%" alt="Microsoft Remote Desktop"/>
</p>
<br />

<p>
So, to recap, here is a shot inside the resourse group with our VM1 inside of it, along with the NIC for VM1, as well as security groups. I made another VM inside of this resource group named VM2 running a linux os. 
<p align="center">
<img src="https://i.imgur.com/aJUX8nR.png" height="80%" width="80%" alt="Microsoft Remote Desktop"/>
</p>

<h2>Congratulations! You have created your first virtual machine within Azure. Azure offers quite a few different options, you could run one VM with Windows, another with Linux, whatever you'd like! It's really quite nice to be able to just create a linux machine, go tinker around in it, play with different interfaces without having to spend thousands of dollars on mulitple different computers just to play with. </h2>
