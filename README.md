# Greenpeace Planet 4 Wordpress
This is not the official repository of the Wordpress.
All credit for the plugin should go to the original author:

	https://wordpress.org/plugins/mappress-google-maps-for-wordpress/

This repository only stores meta information about this plugin, so that it is
usable via Composer in the Planet 4 project.

To install this plugin add the Planet 4 registry to your `composer.json`:

	"repositories": [{
		"type": "composer",
		"url": "https://planet4.greenpeace.org"
	}],

and the dependency to the require section:

	"require": {
		"greenpeace/wordpress": "4.7.2"
	}


## Updating
To update Wordpress to a new version three things need to be changed inside 
the `composer.json`:

1. Update the version number to the new one of the core
2. Update the repository information with the updated download and source path
3. Update the dependency of this package to the new upstream version.

After the changes are commited, a new tag with the same version is created (e.g. 
`v4.7.2`) and pushed to the repository, the continuous integration server 
should build a new version of Wordpress automatically. 
