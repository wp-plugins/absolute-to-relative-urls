=== Absolute-to-Relative URLs ===
Author: Steven Vachon
URL: http://www.svachon.com/
Contact: prometh@gmail.com
Contributors: prometh
Tags: absolute, function, link, links, plugin, relative, shorten, url, urls
Requires at least: 3.1
Tested up to: 3.1
Stable tag: trunk

A FUNCTION for use in shortening URL links. This plugin is meant for dev work and does not automatically shorten URLs.


== Description ==

**PHP 5.2 required.**

Before:
http;//example.com/wp-content/themes/twentyten/style.css

After:
/wp-content/themes/twentyten/style.css

If you are looking for a plugin that *automatically* converts absolute URLs to relative URLs, check out my other plugin **[WP-HTML-Compression](http://wordpress.org/extend/plugins/wp-html-compression/)** as it will soon have this feature.

I wrote this plugin because I needed a basepath for an Adobe Flash application. In other words, I needed a URL to the server root without the domain. You may find this useful for the same reason, or perhaps another.

**Before you copy this code and add it into your code**, keep in mind that there may be future updates. Keeping the code within an activated plugin is often safer.

If you are looking for a solution to WordPress inserting absolute media URLs into your posts, you may want to check out **[Relative Image URLs](http://wordpress.org/extend/plugins/relative-image-urls/)**. 


== Installation ==

1. Download the plugin (zip file).
2. Upload and activate the plugin through the "Plugins" menu in the WordPress admin.


== Frequently Asked Questions ==

= Why isn't this automatic? =

Check out **[WP-HTML-Compression](http://wordpress.org/extend/plugins/wp-html-compression/)**.

= How does this work? =

Just use `absolute_to_relative_url($url)`.

= Will this plugin work for WordPress version x.x.x? =

This plugin has only been tested with versions of WordPress as early as 3.1. For anything older, you'll have to see for yourself.

= Why do you only support a minimum of PHP 5.2? =

It offers substantial improvements over earlier PHP 5 releases, and WordPress 3.2 will not be supporting anything less.


== Screenshots ==


== Changelog ==

= 0.1 =
* Initial release