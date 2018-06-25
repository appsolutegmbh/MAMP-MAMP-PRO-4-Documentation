---
title: MAMP PRO (Mac) Documentation > How Tos > MySQL
description: 
layout: default-2
product: MAMP PRO Mac
language: en
---

### Install and run MongoDB

It is possible to install and use MongoDB along with MAMP PRO PHP. Installing and running MongoDB takes several steps.

<div class="alert" role="alert">
Note: We cannot provide support for installing or maintaining MongoDB.
</div>

---

First compile a mongoDB extension using PECL. We have a How-To guide on how to compile your own [mongoDB extension](http://documentation-4.mamp.info/en/MAMP-PRO-Mac/How-Tos/General/PECL/){:target="_blank"}.

---

Download the [MongoDB Community Edition](https://www.mongodb.com/download-center#community){:target="_blank"}. After downloading you should find a mongodb-osx-xxxx.tgz file. Uncompress this file and you should have the following directory structure. 

![MAMP](/en/MAMP-PRO-Mac/How-Tos/MySQL/InstallMongoDB/mongoDBStructure.png)

Move your mongodb-osx-ssl-xxxx directory to `/usr/local`, resulting in `/usr/local/mongodb-osx-ssl-xxxx`. Create a  `/data/db` directory to hold your MongoDB data. This is the default location for MongoDB data. Additional installation instructions can be found [here](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/){:target="_blank"}.

---

Open a terminal window to run MongoDB. Navigate to `/usr/local/mongodb-osx-ssl-xxxx/bin` directory and type the following to start your MongoDB server.
  
  {% highlight php %}
  ./mongod 
  {% endhighlight %}
  
---

In addition to the MongoDB extension you will need the MongoDB library. Use Composer to install the MongoDB library. Information on downloading composer can be found [here](https://getcomposer.org/doc/00-intro.md){:target="_blank"}. Scroll down and click on  "download this file" for OS X. This should download an "Installer" file to your downloads folder. 

Next create a host. In a new terminal navigate to the document root of   your new host. Move the Install file which you downloaded from the Composer website to your document root. Run the following commands in your terminal found in the Composer documentation as explained [here](https://getcomposer.org/download/){:target="_blank"}.
 
 {% highlight php %}
  php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
    php -r "if (hash_file('SHA384', 'composer-setup.php') === '669656bab3166a7aff8a7506b8cb2d1c292f042046c5a994c43155c0be6190fa0355160742ab2e1c88d40d5be660b410') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
  php composer-setup.php
  php -r "unlink('composer-setup.php');"
 {% endhighlight %}
  
 Type the following in your terminal and press return.
    
 {% highlight php %}
  php composer.phar require mongodb/mongodb
 {% endhighlight %}
     
 Your document root should now look like the following.
    
    
![MAMP](/en/MAMP-PRO-Mac/How-Tos/MySQL/InstallMongoDB/documentRoot.png)
    
---

Once you have installed this, you can use the following [code example](http://php.net/manual/de/mongodb.tutorial.library.php){:target="_blank"} to insert into your new MongoDB database.

{% highlight php %}

require 'vendor/autoload.php'; // include Composer's autoloader

$client = new MongoDB\Client("mongodb://localhost:27017");
$collection = $client->demo->beers;

$result = $collection->find( [ 'name' => 'Hinterland', 'brewery' => 'BrewDog' ] );

foreach ($result as $entry) {
    echo $entry['_id'], ': ', $entry['name'], "\n";
}

{% endhighlight %}



