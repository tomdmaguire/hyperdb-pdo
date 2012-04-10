** Info

This is a (work in progress) merge of Hyper DB (http://wordpress.org/extend/plugins/hyperdb/) with PDO for Wordpress (http://wordpress.org/extend/plugins/pdo-for-wordpress/)

Mysql is currently working, but the sqlite implementation still requires work

** Installation

By default it will use the mysql implementation by this can be overwritten by adding the following to your wp-config.php file:
define('DB_TYPE', 'sqlite');

1. Enter a configuration in db-config.php.

2. Deploy db-config.php in the directory that holds wp-config.php. This may be the WordPress root or one level above. It may also be anywhere else the web server can see it; in this case, define DB_CONFIG_FILE in wp-config.php.

Deploy db.php, PDOEngine.php and the driver_sqlite folder to the /wp-content/ directory. Simply placing this file activates it. To deactivate it, move it from that location or move the config file.
