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

Once Directory setup successfully, we can proceed to provision LAMP Container stack
