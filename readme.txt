=== Absolute-to-Relative URLs ===
Author: Steven Vachon
URL: http://www.svachon.com/
Contact: prometh@gmail.com
Contributors: prometh
Tags: absolute, function, link, links, plugin, relative, shorten, url, urls
Requires at least: 3.2
Tested up to: 3.2
Stable tag: trunk

A **function()** for use in shortening URL links. This plugin is meant for dev work and does not automatically shorten URLs.


== Description ==

If you were to run this code at *http;//example.com/test/testing/*, you would get these results:

* **Before:** http;//example.com/test/another-test/#anchor
* **After:** ../another-test/#anchor
,
* **Before:** http;//example.com/wp-content/themes/twentyten/style.css
* **After:** /wp-content/themes/twentyten/style.css
,
* **Before:** http*s*;//example.com/wp-content/themes/twentyten/style.css
* **After:** http*s*;//example.com/wp-content/themes/twentyten/style.css
,
* **Before:** http;//google.com/test/
* **After:** http;//google.com/test/
,
* **Before:** ../../../../../../../../#anchor
* **After:** /#anchor
* **After** (`$choose_shortest_path=false`)**:** ../../#anchor

***All string parsing. No directory browsing.***

If you're looking for a plugin that will automatically convert *all* of the absolute URLs on your pages to relative URLs, check out my other plugin **[WP-HTML-Compression](http://wordpress.org/extend/plugins/wp-html-compression/)** as it has integrated this code.

**Before you copy this code and add it into your own**, keep in mind that there will probably be future updates. Keeping the code within an installed plugin will make sure you're notified.


== Installation ==

1. Download the plugin (zip file).
2. Upload and activate the plugin through the "Plugins" menu in the WordPress admin.


== Frequently Asked Questions ==

= Why isn't this automatic? =

Check out **[WP-HTML-Compression](http://wordpress.org/extend/plugins/wp-html-compression/)**.

= How does this work? =

Just use `absolute_to_relative_url($url)`.

= Will this plugin work for WordPress version x.x.x? =

This plugin has only been tested with versions of WordPress as early as 3.2. For anything older, you'll have to see for yourself.


== Changelog ==

= 0.2 =
* Parenting (`../`) now supported for both input and output
* Differentiates protocols, usernames, passwords, hosts, ports, paths, resources, queries and fragments/hashes
* Considers domains with and without "www." to be identical, and can be overridden
* Outputs the shortest url (absolute or relative) by default, and can be overridden
* Custom site URL support, but only with a separate `new Absolute_to_Relative_URLs()` instance

= 0.1 =
* Initial release