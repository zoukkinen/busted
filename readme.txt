=== Busted Fenix===
Contributors: zoukkinen & pdclark
Plugin URI: https://github.com/zoukkinen/busted-zoukkinen/
Orginal Plugin URL: https://github.com/pdclark/busted
Orginal Author URI: http://pdclark.com
Tags: browser cache, develop, debug, client, clear, empty, refresh
Requires at least: 4.0
Tested up to: 5.2.2
Stable tag: 1.7
License: GPLv2
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Force browsers to load the most recent file if modified.

== Description ==

Saves you from asking "have you emptied your cache?". And forces the "style.css?v.1.1.1" to update if file is changed.

**Features**

* Safe to leave running on live sites.
* Only refreshes browser cache for a file if it has been modified.
* Resolves Content Delivery Network (CDN) issues. No need to purge CDN cache.
* Multisite compatible.
* "Just works" — no configuration necessary.

**Requirements**

Requires scripts use any of the below functions to load. Almost all files meet these requirements. The only case it doesn't account for is when URLs are hard-coded. This shouldn't ever be done, since it can break sites for other reasons.

* [wp_enqueue_style](http://codex.wordpress.org/Function_Reference/wp_enqueue_style)
* [wp_enqueue_script](http://codex.wordpress.org/Function_Reference/wp_enqueue_script)
* [get_stylesheet_uri](http://codex.wordpress.org/Function_Reference/get_stylesheet_uri)

Photo credit: [Brent Schneeman](http://www.flickr.com/photos/schneeman/3286137238/) – [cc](http://creativecommons.org/licenses/by-nc/2.0/)

== Installation ==

1. Install Plugin as zip-file.
1. Install the plugin.
1. Activate the plugin.

== Changelog ==

= 1.7 =
* Search and replace for wp_print_scripts to wp_enqueue_scripts

= 1.6 =
* Rename slug to match new plugin naming 

= 1.5 =
* Fix: Edit PHP_INIT_MAX - action wp_print_scripts to wp_enqueue_scripts

= 1.4 =

* Fix: Enable for stylesheets, not just JavaScript. Thanks [@francescolaffi](https://github.com/pdclark/busted/issues/5).
* Fix: Enable in wp-admin. For real this time.
* Fix: Hopefully suppress mysterious notice on login screen. Thanks @norcross.

= 1.3 =
* New: Change version slug to 'b-modified' to avoid user confusion.

= 1.2 =
* New: Enable in wp-admin. Thanks @norcross.

= 1.1 =
* New: Only refresh cache if file has been modified. Thanks [@unserkaiser](https://twitter.com/unserkaiser/status/402995947430375424).

= 1.0 =
* Initial public release.

== Upgrade Notice ==
= 1.7 =

* Fix: Depricated function in the plugin. Thanks to [@timstl](https://github.com/pdclark/busted/pull/9) for the fixing PR in the orginal repository.

= 1.4 =

* Fix: Enable for stylesheets, not just JavaScript. Thanks [@francescolaffi](https://github.com/pdclark/busted/issues/5).
* Fix: Enable in wp-admin. For real this time.
* Fix: Hopefully suppress mysterious notice on login screen. Thanks @norcross.
