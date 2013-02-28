wpWizard
=================

*wpWizard has been renamed!*

wpWizard automates the set up a WordPress install complete with theme framework of your choice, a git repository with an empty initial commit (for easy rebasing), plugins of your choice, database creation and creation of wp-config file complete with unique RSA salts.

Who it's for
============

This is primarily for developers that need to set up WordPress installations quite frequently and have gotten annoyed at spending time on automatable actions.


What it automates
============

* Downloads and extracts WordPress
* Configures DB information
* Installs or copies your starter theme or framework. Currently includes [Blue Ox](http://github.com/AaronHolbrook/Blue-Ox.git), [_s](http://github.com/Automattic/_s.git), [Starkers](http://github.com/viewportindustries/starkers.git), [BootstrapWP](http://github.com/rachelbaker/bootstrapwp-Twitter-Bootstrap-for-WordPress.git), [HTML5](http://github.com/murtaugh/HTML5-Reset-Wordpress-Theme.git), [StartBox](http://github.com/brichards/StartBox.git), [Bones](http://github.com/eddiemachado/bones.git), [Roots](http://github.com/retlehs/roots.git), [Reverie](http://github.com/milohuang/reverie.git), [Required](http://github.com/wearerequired/required-foundation.git), [Thematic](http://github.com/ThematicTheme/Thematic.git), [Skeleton](http://github.com/simplethemes/skeleton_wp.git), [WP-Talon](http@github.com:dustyf/wp-talon.git), or any local or remote Git repository.
* Removes the Hello, Dolly! plugin
* Downloads or installs your favorite plugins
* Sets up a git repository, with commits during all stages of installation


Requirements
===========

* Mac OS X >= 10.5
* MAMP or MAMP Pro
* `Bash` >= 3.2



Installation
=======
Simply run `brew tap bradp/wpwizard` and then `brew install wpwizard`.

**If you don't have homebrew installed:** Place the folder within your Bash path (`/usr/local/sbin/`, `/usr/local/`) or add it to your Bash profile path.



Running
=======

Via the command line, navigate to your desired placement of your new WordPress install, simply run `wpwizard`. 

`wpwizard` optionally accepts one or two arguments on the command line, which is the intended name of your project. This argument is used to create the database name, theme folder and the table prefix. The second is the name of the framework. 

Example usage: `$ wpwizard` . All options will be asked when running.

Advanced usage: You can feed the framework name in as well so `$ wpwizard www mywwpinstall skeleton` would create a database and theme folder named 'mywpinstall', using Skeleton as a framework in the `www` directory.

Enjoy your new WordPress install!

Customizing Plugins
===================

Simply add or remove the slug of the plugins you want wpWizard to install to the `conf/plugins.conf` file!

Thanks!
===================

Thanks to [Aaron Holbrook](http://a7web.com) for originally writing wpbuildr - the project this was forked from. 
