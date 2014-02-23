# Installation


Mockery may be installed using Composer, PEAR or by cloning it from its GitHub repository.
These three options are outlined below.


## Composer

You can read more about Composer and its [main repository](https://github.com/composer/composer).
To install Mockery using Composer, first install Composer for your project using the instructions
on the [Packagist](https://packagist.org) home page. You can then define your development
dependency on Mockery using the suggested parameters below. While every effort is made to keep
the master branch stable, you may prefer to use the current stable version tag instead.

    {
        "require-dev": {
            "mockery/mockery": "dev-master@dev"
        }
    }

To install, you then may call:

    composer.phar install --dev

This will install Mockery as a development dependency but will not install it
for regular non-development installs.


## PEAR

Mockery is hosted on the [survivethedeepend.com](http://pear.survivethedeepend.com) PEAR channel and
can be installed using the following commands:

    sudo pear channel-discover pear.survivethedeepend.com
    sudo pear channel-discover hamcrest.googlecode.com/svn/pear
    sudo pear install --alldeps deepend/Mockery


## Git

The git repository hosts the development version in its master branch. You can
install this using Composer by referencing dev-master as your preferred version
in your project's composer.json file as the earlier example shows.

You may also install this development version using PEAR:

    git clone git://github.com/padraic/mockery.git
    cd mockery
    sudo pear channel-discover hamcrest.googlecode.com/svn/pear
    sudo pear install --alldeps package.xml

The above processes will install both Mockery and Hamcrest.
While omitting Hamcrest will not break Mockery, Hamcrest is recommended
as it adds a wider variety of functionality for argument matching.
