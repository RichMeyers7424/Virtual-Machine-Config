# Virtual-Machine-Config
<p align="center">
<img src="https://i.imgur.com/7AUG74j.png" height="40%" width="40%" alt="Microsoft Azure Logo"/>
</p>

<h1>Deploy a Virtual Machine in Azure</h1>
Microsoft Azure is a cloud computing platform with numerous products and services. This guide will demonstrate how to create an account, utilize the portal, and create a virtual machine.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure
- Microsoft Remote Desktop (macOS) for virtual machines

<h2>Configuration Steps</h2>

- Step 1: Create Azure Account
- Step 2: Azure portal and resource group
- Step 3: Create a virtual machine
- Step 4: Connect to virtual machine using Microsoft Remote Desktop on macOS

<h3>Step 1: Create Azure Account</h3>
First step is to create an Azure account. You can create an account with $200 of free credit for a month. 

<br>
<br>

<p align="center">
<img src="https://i.imgur.com/8NgUUZu.png" height="80%" width="80%" alt="Azure Free Account"/>
  

Follow all the prompts to create the account. A credit card will be needed but will not be charged until the $200 credit runs out or the account has been active for a month. After you create your account, you are now a tenant in Azure!

<h3>Step 2: Azure portal and resource groups</h3>

Now that the account has been created, let's go over how to navigate the Azure portal. The portal is where you can find all the products/resources and manage your subscriptions. It is a user friendly interface.

The Azure portal is located [here](https://www.portal.azure.com).

In order to utilize some of the services in Azure, a resource group needs to be created. Resource groups store all resources that you are utilizing in Azure. This example will show how to deploy a Windows 10 virtual machine.

<p align="center">
<img src="https://i.imgur.com/ZwOljpS.png" height="80%" width="80%" alt="Azure Resource Groups with circle"/>
</p>

When ready, click create resource groups. From there, you will need to name your resource group and select the region. The region will determine which Azure data center will be utilize. (US) West 3 was chosen for this example. Click "Review + Create" once finished

<p align="center">
<img src="https://i.imgur.com/lCxkFRI.png" height="80%" width="80%" alt="Create Azure Resource Groups"/>
</p>

<h3>Step 3: Create a virtual machine</h3>
<p>
Now we are ready to create our first Virtual Machine!! To do so, click on the virtual machine tab, then click on create.  A few different options will appear, just chose the Azure virtual machine option. From here, we will be presented with quite a few different options. We will only be using the Basics and Networking sections. Be sure that the virtual machine is placed in the resourse group that you just created. Now we will give our VM a name, this will help us differentiate between multiple VM's running simotanously. Im gonna chooose VM1, basic and generic but effective.
</p>
<p align="center">
<img src="https://i.imgur.com/n61PWNI.png" height="80%" width="80%" alt="Virtual Machine Menu with arrow"/>
</p>

<p>
Next, we will have to choose an operating system. Azure offers quite a few different options, you could run one VM with Windows, another with Linux, whatever you'd like! It's really quite nice to be able to just create a linux machine, go tinker around in it, play with different interfaces without having to spend thousands of dollars on mulitple different computers just to play with. Invaluable. I
</p>
<p align="center">
<img src="https://r.com/a0OIYax.png" height="80%" width="80%" alt="Create Virtual Machine"/>
</p>

<h3>Step 4: Connect to virtual machine using Microsoft Remote Desktop (RDP)</h3>
The final step to this process is accessing the virtual machine using Microsoft Remote Desktop. If you are a macOS user, you have to download the application in the App Store. 

<p align="center">
<img src=" height="80%" width="80%" alt="Microsoft Remote Desktop"/>
</p>

In order to connect to the virtual machine, you will need the public IP address. You can find this on the right hand side of this menu.

<p align="center">
<img src="https://r.com/gT6F62H.png" height="80%" width="80%" alt="SampleVM menu with arrow and circle"/>
</p>

Once Microsoft Remote Desktop is downloaded, open the application. Click add PC. Copy and paste the public IP address of the virtual machine that was created when prompted. Type in the username and password the click connect. 

<p align="center">
<img src="https://r.com/WcRdlX3.png" height="80%" width="80%" alt="Microsoft Remote Desktop 1"/>
</p>

<p align="center">
<img src="https://r.com/4IKJFik.png" height="80%" width="80%" alt="Windows 10 VM"/>
</p>

Congratulations! You have created your first virtual machine within Azure. If you want to save your free $200 credits, make sure you delete ALL resource groups because most of Azure services are pay as you go (unless otherwise stated). Thank you!
