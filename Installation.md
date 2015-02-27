# Installation of TilingScan

**(This guide is only if you want to install and use TilingScan on your computer. If not, you can use TilingScan [here](http://tilingscan.uv.es))**

Here we describe the steps to install a local copy of TilingScan on your Ubuntu/Debian localhost. 

In this guide we assume that you have a minimum knowledge of Linux commands.

## Step 1: install Apache

First, you must install **Apache** on your computer. For this, open a terminal and write:

```
sudo apt-get install apache2 -y
```

You can check if **Apache** is now working opening this url: http://127.0.0.1

## Step 2: install PHP

Because TilingScan is written in **PHP**, you need to install the **PHP libraries** to work with TilingScan. Execute this command in a terminal:

```
sudo apt-get install php5 libapache2-mod-php5 -y
```

And restart the **Apache** service:

```
sudo /etc/init.d/apache2 restart
```

We recommend install this other modules for **PHP**:

```
sudo apt-get install php5-mysql php5-curl php5-gd php5-idn php-pear php5-imagick php5-imap php5-mcrypt php5-memcache php5-ming php5-ps php5-pspell php5-recode php5-snmp php5-sqlite php5-tidy php5-xmlrpc php5-xsl -y
sudo /etc/init.d/apache2 restart
```





