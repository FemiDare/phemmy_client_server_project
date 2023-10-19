# phemmy_client_server_project

I used the curl command to send a request to a webserver for the site www.propitixhomes.com

![Screenshot 2023-10-14 164032](https://github.com/FemiDare/phemmy_client_server_project/assets/140294606/ff9abe3a-5fee-4e5e-9470-f2dc82633e47)

I spun two ubuntu instances on my AWS server, one named "mysql_server" and another named "mysql_client"

Connected to each server from two seperate terminal windows and changed the names for the purpose of differentiation 

![Screenshot 2023-10-16 230827](https://github.com/FemiDare/phemmy_client_server_project/assets/140294606/1642cf72-7937-4988-aca1-1925bf50990f)

![Screenshot 2023-10-16 231922](https://github.com/FemiDare/phemmy_client_server_project/assets/140294606/279626e8-d6d7-422a-b973-b343890e40e7)

![Screenshot 2023-10-16 232117](https://github.com/FemiDare/phemmy_client_server_project/assets/140294606/e34138a5-9477-4951-b2f3-55b66107e171)

On the mysql_server terminal I installed mysql-server software and on the mysql_client terminal I installed mysql_client software

![Screenshot 2023-10-17 161052](https://github.com/FemiDare/phemmy_client_server_project/assets/140294606/8616ccaa-1813-4cff-a307-bd56e464b35d)

![Screenshot 2023-10-17 161219](https://github.com/FemiDare/phemmy_client_server_project/assets/140294606/44e0a4f0-4b71-40c6-9f83-7f3df563fe51)

I then went to security groups of the instance mysql_server to edit the inbound rules by opening the TCP port 3306 which is the default port for Mysql

![Screenshot 2023-10-17 161350](https://github.com/FemiDare/phemmy_client_server_project/assets/140294606/4b6176ca-b79c-4fda-a3c6-ed39c2502326)

I editted the mysqld.cnf file using the vi command by changing the binding-address from 127.0.0.1 to 0.0.0.0 

![Screenshot 2023-10-17 161504](https://github.com/FemiDare/phemmy_client_server_project/assets/140294606/b104b0cb-76fc-49dd-a395-d1811546c70e)

![Screenshot 2023-10-17 161536](https://github.com/FemiDare/phemmy_client_server_project/assets/140294606/cb6af85f-cd76-4825-9795-c9330db358c5)

I then connected to mysql_server database engine from mysql_client linux server remotely and tested that the connection was made successfully 

![Screenshot 2023-10-17 162721](https://github.com/FemiDare/phemmy_client_server_project/assets/140294606/6ae5a973-8c7a-4abd-8598-226fdbc36fec)

![Screenshot 2023-10-17 163050](https://github.com/FemiDare/phemmy_client_server_project/assets/140294606/691e4195-1265-4daa-8f24-33df3f51c938)

![Screenshot 2023-10-17 163109](https://github.com/FemiDare/phemmy_client_server_project/assets/140294606/b28eac29-e5d1-4029-a900-f58406154c79)
