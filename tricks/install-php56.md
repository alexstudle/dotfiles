# Install PHP 5.3 (or 7.x)

we have to add specific repositories

```
sudo add-apt-repository ppa:ondrej/php
sudo apt-get update
```

then install php5.6 (or another version) with modules
```
sudo apt-get install php5.6 php5.6-mysql php-gettext php5.6-mbstring php-mbstring libapache2-mod-php5.6
```

## And to switch between versions
### CLI
```
sudo update-alternatives --set php /usr/bin/php5.6
```

### Apache
```
sudo a2dismod php7.0 ; sudo a2enmod php5.6 ; sudo service apache2 restart
```
