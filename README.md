Fetch File
==========

Fetch File makes it easy to download libraries you require very often directly from the command line.

By [Florian Eckerstorfer](http://florianeckerstorfer.com) (@[Florian_](http://fleckr.com/twitter)).

Usage
-----

View a list with all available packages

	$ php ~/ff
	silex: http://silex.sensiolabs.org/get/silex.phar
	jquery: http://code.jquery.com/jquery.min.js
	
Download a package into the current working directory.

	$ php ~/ff silex
	Downloaded silex to "./silex.phar".
	
Download a package into a given directory. The directory must be relative to the current working directory

	$ php ~/ff silex vendor/
	Downloaded silex to "./vendor/silex.phar".
	

Installation
------------

1. Download the `ff` file  and place it in a directory where you can easily reach it. I choose my user directory `~`.
2. Create a file `.fetchfile` in your user directory.
3. Add packages to your `.fetchfile` in JSON format.

A sample `.fetchfile` could look like this:

	{
		"silex": "http://silex.sensiolabs.org/get/silex.phar",
		"jquery": "http://code.jquery.com/jquery.min.js"
	}







