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
  <img/ src = "https://i.imgur.com/dzMZNxt.png" height ="80%" width = "80%" alt= "File Share img"/>
  </p>
    
 <p>  To enable File Sharing and its permissons, fromm a Domian Controller folders to a clients. We first need to create our Folders in the Domain Controller(DC-1)
  All are created in this pc C-Drive. One folder will be "Read Folder" Everyone can access but only read. another, "Write Folder" All can view , write, and create files.These can be given access by everyone by right clicking then clicking on properties. Once we are here we click on Sharing. then press shar button. Once this pressed, we type "Domain Users". Press add. Be sure to set prmission  based on folders.  . Then we will have an admin folder in which only An admin can access. To do this we right click on Admin folder. We then click sharing tab. Once here we Cick share button. Then in presented search bar we rite and press add once "Domain Admins" is Written. Be sure to to click Permission level for this group is Read/Write. 
Lastly, We are making an "Engineer Folder". I will now to only add A ceratin group tom access a certain folder. In our case it being the Engineer Folder.
  </p>
  
   <p>
    <img/ src = "https://i.imgur.com/8zda541.png" height ="80%" width = "80%" alt= "File Share img"/>
    
  </p>
    
 <p> 
 To access the server folders on client-1 we use the seacrh bar in file explore. We type the domain controller host name. In our case "\\dc-1".
  
  </p>
  
  <p>
    <img/ src = "https://i.imgur.com/0y1SiQh.png" height ="80%" width = "80%" alt= "File Share img"/>
    
  </p>
    
 <p> 
  Here we see that a read file was created in DC-1.
  </p>
  
  <p>
    <img/ src = "https://i.imgur.com/KeozTxR.png" height ="80%" width = "80%" alt= "File Share img"/>
    
  </p>
    
 <p> 
 On client one we see that all our files appear. For our example we also read is accessable but Client-1's user cant make anychanges but can view the file.
  
  </p>
  
  <p>
    <img/ src = "https://i.imgur.com/FoCsKZZ.png" height ="80%" width = "80%" alt= "File Share img"/>
    
  </p>
    
 <p> 
Now I will show how we can give only ceatain security group file permissions. First we notice our user jake can't access "Engineer Folder". They need to. So we as an admin in active directory need to create a security group for our engineers. So to do this we right click inn the Organized unit and right click in it and create a "group" it will be named Engineers, for our example. Once added we right click and click member tab.  Then we type in our desired user. In this case jake is the user.
   Then once donme press add to them to the group.
  
  </p>
  
  <p>
    <img/ src = "https://i.imgur.com/OrfZAZx.png" height ="80%" width = "80%" alt= "File Share img"/>
    
  </p>
    
 <p> 
 In DC-1 we have a file to view for our Engineer. 
  
  </p>
  
  <p>
    <img/ src = "https://i.imgur.com/Vf6oq43.png" height ="80%" width = "80%" alt= "File Share img"/>
    
  </p>
    
 <p> 
 Now, as we see, jake can view the folders contents. They can ever edit to, based on the provided permissions of the folder.
  
  </p>
  
