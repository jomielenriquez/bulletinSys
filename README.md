# Bulletin System
>Bulletin System

### :hammer_and_wrench: OS Installation
1. Install the latest ubuntu 20.04 LTS to an SD card using raspberry pi imager and connect the SD card to the raspberry pi
    <div>
      <img src='https://user-images.githubusercontent.com/77730490/195964670-a37b4e39-271e-4608-b31d-fdfc40e02273.png'/>
    </div>
2. Boot the system and update using the code below.
```
sudo apt update && sudo apt upgrade
```
3. Install mysql server using the command below
```
sudo apt install mariadb-server
```
4. After installing the mariadb server. Execute the command below to setup the database.
```
sudo mysql_secure_installation
```
5. After setting up password just select no 'n' in everything in the setup.
6. To access Mariadb, execute the command below.
7. Install the MYSql connector to PHP using the command below.
```
sudo apt install php-mysql
```
8. Install PHP https://pimylifeup.com/raspberry-pi-latest-php/

```
sudo mysql -u root -p
```
### :hammer_and_wrench: Mariabd commands
- Creating new database.
```
CREATE DATABASE <DATABASE NAME>
```
- Creating new user
```
CREATE USER '<USERNAME>'@'localhost' identified by '<PASSWORD>';
```
- Giving acces to a user
```
GRANT ALL PRIVILEGES ON <DATABASE NAME>.* TO '<USERNAME>'@'localhost';
```
### :hammer_and_wrench: Database setup
Database Name: bulletinDb,
User: admin,
Pass: admin








