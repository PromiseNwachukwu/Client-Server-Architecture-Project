# Client-Server Architecture with MySQL
### A typical example of a Client-Server communication.
![Screenshot from 2023-10-04 22-32-07](https://github.com/PromiseNwachukwu/Client-Server-Architecture-Project/assets/109115304/49a5228e-c5aa-401b-a09a-8461f72ca8c4)

## Implementing a Client Server Architecture using MySQL Database Management System (DBMS).
### (1). Create and configure two Linux-based virtual servers (EC2 instances in AWS). 
Server A name - `mysql server`

Server B name - `mysql client`
![Screenshot from 2023-10-05 22-37-24](https://github.com/PromiseNwachukwu/Client-Server-Architecture-Project/assets/109115304/74e8aabd-6bf0-4107-93a9-be830abe0fdb)

### (2). On mysql server Linux Server install MySQL Server software.
![Screenshot from 2023-10-05 10-38-11](https://github.com/PromiseNwachukwu/Client-Server-Architecture-Project/assets/109115304/e8d00f18-9a08-4727-972b-d6e0256e5755)

### (3). On mysql client Linux Server install MySQL Client software.
![Screenshot from 2023-10-05 10-42-14](https://github.com/PromiseNwachukwu/Client-Server-Architecture-Project/assets/109115304/e6859311-25b1-4bad-a4dc-fc1cf4650267)

### (4). Connecting to the Linux Server from the Client.
#### To open TCP port 3306 which is the default port for MySQL server.
![Screenshot from 2023-10-05 10-57-33](https://github.com/PromiseNwachukwu/Client-Server-Architecture-Project/assets/109115304/494561cd-3d6c-4dbf-afe3-75127c6d9eb4)

#### (5). Configuring MySQL server to allow connections from remote hosts. 
sudo vi /etc/mysql/mysql.conf.d/mysqld.cnf 

Replace '127.0.0.1' to '0.0.0.0' like this:
![Screenshot from 2023-10-05 11-09-23](https://github.com/PromiseNwachukwu/Client-Server-Architecture-Project/assets/109115304/67eaa86e-22a3-49b9-80da-aa7b1598b4fd)

#### (6). From mysql client Linux Server connect remotely to mysql server Database Engine without using SSH. You must use the mysql utility to perform this action.
![Screenshot from 2023-10-05 23-18-10](https://github.com/PromiseNwachukwu/Client-Server-Architecture-Project/assets/109115304/4afd94b8-fc32-4237-8b01-5d2369d0e630)

#### (7). Check that you have successfully connected to a remote MySQL server and can perform SQL queries.
![Screenshot from 2023-10-05 23-42-44](https://github.com/PromiseNwachukwu/Client-Server-Architecture-Project/assets/109115304/5b2893e6-d8d9-4327-94c0-a54279f6ecce)

### Project completed.

