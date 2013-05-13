# Drupal Tools

## Configuration file

Default values can be saved in a configuration file (/project.drush.sh/) that is in /.drush/ directory above the 
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

## dn-drup

/dn-drup/ is a command to download a drupal to a local development environment.