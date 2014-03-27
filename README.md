# Drupal Tools

## Configuration file

Default values can be saved in a configuration file (project.drush.sh) that is in *.drush* directory above the 
current directory.

Example:

- my-project/ 
	- .drush/ 
   		* project.drush.sh
	- web/ 
   		* ...drupal install

### Sample config file

		export DRP_LIVE="@myproj.live"
		export DRP_TEST="@myproj.test"
		export DRP_DEV="@myproj.dev"
		export DRP_LOCAL="@myproj.local"
		export BRAVELY_DROP=""
		export RSYNC_OPTIONS="--no-group --exclude=files/xmlsitemap --exclude=.DS_Store"
		export RSYNC_LOCAL="/home/cleaver/projects/web/"
		export RSYNC_SERVER="cleaver@www.example.com:/var/www"

## commands

 - *dn-drup* is a command to download a drupal database to a local development environment.
    
 - *up-rsync* is a command to rsync drupal code from local up to a server. Allows one extra option (probably good to use --dry-run the first time).
