OS-X-Dev-Environment
====================

Notes on creating an OS X native development environment. My primary
goals were to be able to do Drupal 8 development with Xdebug support,
which meant that MAMP wasn't a viable option. I also wanted to do
work in Ruby and make another shot at getting an Xcode environment
for Arudino development going. A secondary goal was to have something
easier to understand than Mark Sonnabaum's Megalodon. Megalodon is
where I'd like to end up, but when it breaks there is a lot to sort
out. I was hoping for something with less of an initial learning
curve.

Drupal Dev Environment Setup Notes
----------------------------------

Based on: http://www.lullabot.com/blog/article/setting-my-mac-without-mamp

Stock Mavericks, plus:

Commercial Tools
----------------
* Xcode command line tools (or full Xcode)
*	Sublime Text
*	PHPstorm

Homebrew
--------

edconf

PHP
---
* Use stock version
*	Copy sample config file /etc/php.ini.default to /etc/php.ini

Apache
------
* Use stock version
*	Enable PHP module
*	Enable clean URLs
*	Enable virtual hosts

MariaDB
-------
brew install mariadb

PostgreSQL
----------
brew install postgresql

Xdebug
------

Drush (https://github.com/drush-ops/drush)
-----
* Use latest for D8 support.

git clone --branch master https://github.com/drush-ops/drush.git

Dreditor (http://dreditor.org)
--------
* Download from project page.
