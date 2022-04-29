# General use

After a (re)boot of your Mac, depending on the setup Apache and MariaDB are already running.
In my personal setup I have to start these manually. I open a terminal and start the services:

```
startdev
```

Apache, MariaDB, DNSMasq and Mailhog are now ready for use.


# Create a new database

- Create a new database with Sequel Ace, DBeaver, Adminer, commandline or whatever tool you user to administrate your MariaDB databases.


# Create a new website

Creating a new website is very simple. In the Sites folder create a new subfolder for your website.

As an example create a folder **testwebsite** or clone a repository in ~/Development/_sites

```
mkdir ~/Development/_sites/testwebsite
```

Then add your html/php/whatever files in the folder ~/Development/Sites/testwebsite.

There is nothing else to configure. The website is immediately ready in your browser at http://testwebsite.test


# Stop Development

Apache, MariaDB, DNSMasq and Mailhog can be stopped with the terminal command:

```
stopdev
```


# Restart development

Apache, MariaDB, DNSMasq and Mailhog can be restarted with the terminal command:

```
restartdev

```

# Reference

## PHP

(replace "< version >" with required PHP-version, 8.1 for example)

### php.ini location

```
code /usr/local/etc/php/< version >/php.ini
```

### Switch to php < version >:

```
sphp <version>
```

### MariaDB default data location

```
/usr/local/var/mysql
```