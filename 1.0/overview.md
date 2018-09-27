#Overview


- [Requirements](#requirements)
- [Getting Started](#getting-started)

Expose is the custom built content management system built by Parallax. It allows you to edit your content within the visible webiste parts rather than a clunky and unclear admin interface.

Expose has transformed into a composer package that is added in to Laravel 5.


<a name="requirements"></a>
### Requirements
To use the Expose Laravel you will need the following:

* PHP 7.0+
* Laravel 5.4+
* Homestead
* Composer
* NPM >= 3.3.12

<a name="getting-started"></a>
### Getting Started
If you haven't already, you need to setup Homestead.

You will need to keep all the Expose Laravel installs in a specific folder for the setup to run fully. Please run the below command to make the needed folder:

```bash
mkdir ~/Code/expose-laravel && cd ~/Code/expose-laravel
```

Next you will need to install the Expose Installer package so that you cen create a new instance of Laravel ready to go with Expose.

To install run the following in your terminal:

```bash
composer global require parallax/expose-installer
```

Once you have done this you are ready to install a new Expose Laravel site