	             ____
	            (____)
	            (____)
	       _______|| 					        WEB1776
	   ___/  _____||_____________/)       _ __  _  _  ___   ____
	  /     /  __________________\)         _   _  __ ___  /	\
	(0)    (  ?__________________ )           _  __ ___   |      |
	  \___  \_____  _____________/)       _ __   ___ ____  \____/
	      \_______||             \)
	             _||_ 				    Revolutionary Web Services
	            (____)
	      		(____)

# Helpers
Contains a list of common helper functions that make building WordPress sites even more fun!

## Functions
**img($uri, $atts = ''):** Creates an image tag. 
Short hand of `<img src="<?php echo get_bloginfo('template_url') . $src ?>" atts=>`. To use, simply do `<?= img('logo.png') ?>`. **Note** This method loads image relative to the `img` directory in our themes folder (just pass in an absolute URL for external images).

**js($uri, $deps = false)** Enqueues a script, relative to the `js` folder in your themes directory to be loaded in the footer. Note that you don't need to add the `.js` extension.

## Auto
Looks in the theme's folder for a favicon named "favicon-admin.$faviconExt", where $faviconExt is the extension (defaults to .ico). To change it to PNG, simply add `$faviconExt = 'png'` to your `functions.php`.