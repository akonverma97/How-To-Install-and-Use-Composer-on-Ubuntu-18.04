# How-To-Install-and-Use-Composer-on-Ubuntu-18.04

# Introduction
Composer is a popular dependency management tool for PHP, created mainly to facilitate installation and updates for project dependencies. It will check which other packages a specific project depends on and install them for you, using the appropriate versions according to the project requirements.
Before you download and install Composer, you’ll want to make sure your server has all dependencies installed.
 
```				
sudo apt update	
```
Now, let’s install the dependencies. We’ll need curlin order to download Composer and php-cli for installing and running it. The php-mbstring package is necessary to provide functions for a library we’ll be using. git is used by Composer for downloading project dependencies, and unzip for extracting zipped packages. Everything can be installed with the following command
		
		
```				
sudo apt install curl php-cli php-mbstring php-curl git unzip 
```
	
 		
With the prerequisites installed, we can install Composer itself.


# Downloading and Installing Composer

```
 curl -sS https://getcomposer.org/installer -o composer-setup.php 
```
To install composer globally, use the following command which will download and install Composer as a system-wide command named composer, under /usr/local/bin:
```
sudo php composer-setup.php --install-dir=/usr/local/bin –filename=composer 
```

You’ll see the following output:
     
Output
All settings correct for using Composer
Downloading...

Composer (version 2.1.9) successfully installed to: /usr/local/bin/composer
Use it: php /usr/local/bin/composer

To test your installation, run:
```   
composer 
```
<img src="composer.png" alt="drawing" width="500"/>




