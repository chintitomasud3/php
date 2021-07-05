# First of all, read the warning! It says do not run composer as root! Secondly, you're probably using Xammp on your local which has the required php libraries as default.
# But in your server you're missing ext-dom. php-xml has all the related packages you need. So, you can simply install it by running:

sudo apt-get update
sudo apt install php-xml


//Most likely you are missing mbstring too. If you get the error, install this package as well with:

sudo apt-get install php-mbstring

//Then run:
composer update
composer require cviebrock/eloquent-sluggable
