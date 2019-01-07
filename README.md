# Docker LAMP

This document describe how to setup LAMP stack with Docker and Container. In this guide, We will setup three Container

o - Apache and php Container

o - MySQL Container

o - PhpMyAdmin Container

**Step 1- Clone git repository to your local machine and change directory**

Run following command to clone reposiory to your local system.
```
git clone https://github.com/amarsingh3d/Docker-LAMP.git
```
**Change Directroy**
```
cd Docker-LAMP
```

**Step 2- Setup prerequisites:**

Before, we provison our LAMP container environment. First, We need to complete some prerequisites.
1-We will setup Two Directories, One for DocumentRoot and Second for MySQL database directory.
  Run the following command to setup two directories. 
```
sh setupdir.sh
```
Copy phpinfo.php to DocumentRoot
```
cp phpinfo.php DocumentRoot
```


Once Directory setup successfully, we can proceed to provision LAMP Container stack

**Step 3- Install docker-compose:**

We need to install docker-compose if it's not already setup. follow the command below to finish the installation.
```
curl -L "https://github.com/docker/compose/releases/download/1.23.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```
Make docker-compose executable
```
chmod +x /usr/local/bin/docker-compose
```

**Step 4- Setup Container LAMP stack:**

To provison LAMP stack run following command.
```
docker-compose up
```

Validate Created Container:
```
docker ps
```
