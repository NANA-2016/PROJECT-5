# PROJECT-5

## Understanding client server architecture Mysql

## Client server Architecture .

A machine  trying to get access to the web  site using a web browser  using the curl command on its owmn terminal is the client  for instance 

$ curl -Iv www.propitixhomes.com for propitixhomes . Kindly see the below screenshot for the request made by the client on its server .

![curl propitixhomes](https://github.com/NANA-2016/PROJECT-5/assets/141503408/1bed9da5-4546-449e-a633-bfddf071ba87)

## Configuring and creating  mysql server and mysql client.

  These is done on AWS cloud by creating instances . 

See the screenshot below to see the 2 servers on AWS.

![Servers created ](https://github.com/NANA-2016/PROJECT-5/assets/141503408/61d63c09-eb07-4484-a5f4-2d61aeb0d504)

## Creating MYSQL Servers Software.

 MYSQL Client

![mysql client server](https://github.com/NANA-2016/PROJECT-5/assets/141503408/3196e1b9-0f04-4575-b300-72fe503cc211)

MYSQL Server .

![mysql server server](https://github.com/NANA-2016/PROJECT-5/assets/141503408/be70e946-a52c-41aa-a951-94e3630031d8)

 To allow communication of both server , we have to set a default TCP  port 3306 by creating a new entry on inbound rules
 
 using private ip address of the server . This is also for security purposes.

 ![changing inbound rules](https://github.com/NANA-2016/PROJECT-5/assets/141503408/bb87ebbd-f0e7-47b3-bc52-02505b66ba85)

 ## Mysql server confuguration.

  We need to configure Mysql server  to allow connectons from to client to the remote host.

   The followng command 'sudo vi /etc/mysql/mysql.conf.d/mysqld.cnf 'and configuratin results are as shown below 
   
   ![mysql server server](https://github.com/NANA-2016/PROJECT-5/assets/141503408/a0775ceb-03a3-4c08-9f97-e7617df0c561)

    To allow mysql client to connect to the server remotely, We have to give the user permissions using mysql commands as 
    
    shown on the screen shot below on the server .
    
![user permissions](https://github.com/NANA-2016/PROJECT-5/assets/141503408/771fe19e-6fdb-45dd-a87e-3c6cd664ce50)

 Lastly we need to test if  the client server can connect sucessfully  to the remote MYSQL server and can perform SQL 
 
 queries. 

  using the trigger commands as shown below on the  screen shots  consecutively.
 
![successful connection to Mysql server  by client prompt](https://github.com/NANA-2016/PROJECT-5/assets/141503408/e226ae71-3b38-47d3-86a2-36b3c4c6e0b8)

![successful connection to Mysql server  by client prompt (2)](https://github.com/NANA-2016/PROJECT-5/assets/141503408/3f3a9e23-42d4-412a-b8c8-cb87baa8ab5c)



 

    

    


   


 




