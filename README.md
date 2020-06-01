OSCOMMERCE 2.3 REMIBIT MODULE

INSTALLATION AND CONFIGURATION

In order to install the module, it is necessary to access the server where the web files are hosted by ssh. If you don’t know how to do that, please contact your site administrator or your hosting provider.

In this example we will use the default oscommerce configuration, so the website files are located in /var/www/html/oscommerce and they are owned by the default user www-data. Please replace [oscommerce] with the actual name (if different) of your website directory and [www-data] with the owner (if different) of your web files directory.

## Requirements

* A RemiBit merchant account
* oscommerce 2.3 (2.3.4.1 recommended)


## Installation

1/. Go to the oscommerce directory

```
cd /var/www/html/oscommerce
```

2/. Fetch the RemiBit module

```
sudo -u www-data wget https://github.com/RemiBit/oscommerce23-remibit/releases/download/v1.01/oscommerce23-remibit.zip
```

3/. Uncompress it

```
sudo -u www-data unzip oscommerce23-remibit.zip
```

Please make sure you are on your {WEBROOT} directory before uncompressing. From it, you should be able to see the README.md file and catalog and docs directories.

The RemiBit module is now in place and prepared to be installed.

4/. Login to Admin dashboard, go to Modules > Payment and click on Install Module button in the top right. 

Scroll down until you find RemiBit Payment Method and select it.

Click on Install Module button. The module will not load until it is configured.


## Configuration

Click on the Edit button and fill up the RemiBit authentication information from your RemiBit merchant account's Settings > Gateway:

* API Login ID
* API Transaction Key
* Signature Key
* MD5 Hash


