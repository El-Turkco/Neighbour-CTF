# Neighbour-CTF
Neighbour-CTF solution

Hello Fridens, Today I will show you the neighbour ctf solution from Tryhackme. 

Lets go first NmapScann

![NmapScan](https://user-images.githubusercontent.com/103064152/227618610-b6d35e76-4ae7-45f5-9bc1-b1ff1c322fe4.png)

 Two opens Port "ssh" and "http" Then later go to web site.
 
 
 ![Web Page1](https://user-images.githubusercontent.com/103064152/227619453-3b2c8d62-b21e-43ce-bb9b-c7c5219e8d5f.png)

We get the login page,Then we do web research,Here I'm using the "dirbuster" tools.

![Enumeration](https://user-images.githubusercontent.com/103064152/227620718-48e44f98-697d-480b-8e4a-1260c4117a28.png)

First the "/db.php" page stands out,go to "http://targetİp/db.php" but  will not response page

Then later go to "login.page" view source.

![web view source](https://user-images.githubusercontent.com/103064152/227622678-05836e09-f4b5-4a8a-9546-d28da0277312.png)

In the source code it tells us to login as guest.Okey go to  back the login page username:guest and password:guest

![login](https://user-images.githubusercontent.com/103064152/227624102-d408d395-3bdc-42bb-a34f-da5782e4c241.png)

![Guest](https://user-images.githubusercontent.com/103064152/227624137-511df743-556a-42fd-969f-f51dbd5dc01c.png)

Manipulation the url part here:"http://Targetİp/profile.php?user=guest" change the user values "admin" then later go to flag page. 

![Admin Flag](https://user-images.githubusercontent.com/103064152/227625205-7c8fc8cf-40e1-4f66-9089-c1ab99840d12.png)
