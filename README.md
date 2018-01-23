1. Environment:
Windows 7 or 10 64Bit
Java 1.8


2. download and install vcredist_x64.exe (Microsoft Visual C++ 2013 Redistributable (x64) - 12.0.40660) from 
https://www.microsoft.com/en-ca/download/details.aspx?id=40784

3. Download mysql-installer-community-5.7.20.0.msi (mysql) from:
https://dev.mysql.com/downloads/windows/installer/5.7.html

4. Install mysql
4.1 Select server only

4.2 Use the default settings. remember the port number. This will be used by client to connect to the server.

4.3 Set password for "Root" user,

4.4 Add users. They can log into the booking database and do the reservation.  

5. After mysql installation, run "MySQL Command Line Client"

6. The password is the password of the "Root" user.

7. Create a new database and tables
7.1 Create a new database
Create database LDHBooking;
7.2 Switch to this DB
use LDHBooking;
7.3 Create 4 tables
Create table block (weekdaynumber int, blockname varchar(30), pos int);
Create table calendar (schoolday date);
Create table carts (Cart_column varchar(40));
Create table reservations(schoolday date, blockname varchar(40), cart_column varchar(100), reservation varchar(40));
 
8. Add data into 3 tables

Insert into block (weekdaynumber, blockname, pos) values(0, 'Block B 8:55-10:10', 1);

See the pic for all data.

Insert into calendar (schoolday) values ('2018-01-08');
Add the required days

Insert into carts (Cart_column) values ('CoCo Lib ChromeChart ChromeCart'); 
Add all required carts

