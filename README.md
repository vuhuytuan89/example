# Create user
@:~$ sudo useradd -m deploy
+ sudo su - deploy
# Run ssh-keygen & add key to github
+ ssh-keygen -t rsa
+ cat ~/.ssh/id_rsa.pub (coppy to github account)
# add key ssh to authorized_keys
touch .ssh/authorized_keys

# 1. Install nginx
## Install

```
    sudo apt-get install nginx
```
# 2. Install PHP-FPM
## Install

```php7.0
sudo apt-get install software-properties-common
sudo add-apt-repository ppa:ondrej/php

    sudo apt-get install  php7.0-cli \
    php7.0-common \
    php7.0-curl \
    php7.0-json \
    php7.0-xml \
    php7.0-mbstring \
    php7.0-mcrypt \
    php7.0-mysql \
    php7.0-zip \
    php7.0-gd \
    php7.0-fpm \
    php7.0-dev 
```
```php7.2
sudo add-apt-repository ppa:ondrej/php
then
apt-get update
apt-get -y install unzip zip nginx php7.2 php7.2-mysql php7.2-fpm php7.2-mbstring php7.2-xml php7.2-curl php7.2-zip
```

# 3. Install MySQL Server & client

## MySQL Server (Client included)

```
    sudo apt-get install mysql-server
```

## MySQL Client (only)

```
    sudo apt-get install mysql-client
```
# 6. Install NodeJS
## NodeJS 9.x
```
    curl -sL https://deb.nodesource.com/setup_9.x | sudo -E bash -
    sudo apt-get install -y nodejs
```
