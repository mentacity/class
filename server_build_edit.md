# Document a LAMP setup and Save the Image
---

## Part I: Setup Local and Remote Repository
---

### Create a Local Git Repo
- Create a new repo on your laptop called docs
	1. Create a folder called docs
	2. cd to docs
	3. run the command: git init to initialize the repository
	4. copy this document into the repo
	5. run: git status
	6. run: git add *
	7. run: git commit -m "First commit with lab guide"
---

### Create a New GitHub Repository Called lamp_server_setup
- Make sure the repository is created empty
- Copy the url of the new GitHub repo
   1. 
---

### Connect Your Local Repo To Your GitHub Repo
- git remote add origin http://pathto/lamp_server_setup.git
- git push -u origin master
---

### Check Your GitHub Repo
- create a new directory elsewhere called test_lamp
- git clone <path_to_your_repo]
- does your new directory contain 
---

### Demo to Instructor Part I is complete

## Part II Setup an Image in the Cloud (Digital Ocean Droplet)
- Guide: https://www.digitalocean.com/community/tutorials/initial-server-setup-with-centos-7
---

### Create a Droplet and Reset the Root Password
- Create a new droplet
- Use SSH to login as root (use the emailed root password)
- Change the root password
- Write down the root password
- Confirm to instructor you can log in and out with the root password
---

### Add a Second User
- Add a second user and set the password 
- adduser <username> passwd <username>
- write down the username and password
- login and backout to test the username
---

### Create SSH Keys Locally and Install Public Key on the server
- Create SSH keys locally
- Copy the public to your new server
- Ensure you can login to your new user with the SSH key
- Disable the root login
---

## Part III Install Apache, MySQL, and Php
- Guide: https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-centos-7
- Install Apache with yum
- Install MySQL with yum
- Secure your MySQL installation
- Install a base Php (you do not have to install the addtional modules)
- You should not have to configure the firewall
- Create Hello World php script (hw.php)
---

## Part IV Creating a Snapshot of your image
- Using the terminal shutdown your server
- Using the Digital Ocean Interface Create a Snapshot of Your Server
- Name it LAMPwithKeys
---

## Part V Install Wordpress
- Guide: https://www.digitalocean.com/community/tutorials/how-to-install-wordpress-on-centos-7
- Do you need wget ? yum install wget
- Test Wordpress
- Create Another Snapshot call it WordPressImage
---

## Part VI Add Encryption with OpenSSL
- Guide: https://www.digitalocean.com/community/tutorials/how-to-create-a-self-signed-ssl-certificate-for-apache-in-ubuntu-16-04
- The guide is for Ubuntu, but should work for CentOS
- Create a final snapshot called WPwithEncryption
---

## Part VII
- Create a new droplet based on your final snapshot 
- Test your WordPress and Encryption by browsing to https://your_ip_address
---


