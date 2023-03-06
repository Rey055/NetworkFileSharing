# NetworkFileSharing


<p align="center">
<img src="https://neroknowhow.com/wp-content/uploads/2021/12/1.png" alt="File Sharing Visualization"/>
</p>




<h2> Network File Sharing</h2>



<h2>Technologies and Envirnoments used <h2>
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Windows 10 Server

<h2>Operating Systems</h2>
-Windows 10 Virtual machine
-Windows 10 Server (Active Directory Installed)


<p>
  <img/ src = "https://i.imgur.com/j4L9yBj.png" height ="80%" width = "80%" alt= "Active Directory img"/>
  </p>
    
 <p>   Using microsoft Azure. I have created two Virtual machines. ONe our data Server named "DC-1" this is where our main windows server will be on. The other being "Client-1 " this client being our test cimputer to connect to our server that will contain Active directory. Now will need to test traffic for both the Client to DC.
  </p>
  
   <p>
  <img/ src = "https://i.imgur.com/FeHYRvE.png" height ="80%" width = "80%" alt= "Active Directory img"/>
  </p>
    
 <p>   First, Logging on to Client-1 we will need to ping Dc-1. We notice that no specfic traffic is reaching from client to DC.
    we staart noticing by defualt ICMP4 traffic cannot be eastibalished from our DC-1(10.0.0.4). Now we need to enable this traffic in our DC-1
  </p>
