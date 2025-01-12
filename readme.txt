=== Remove Category Base ===

Contributors: littlebizzy
Donate link: https://www.patreon.com/littlebizzy
Tags: remove, disable, category, base, permalinks
Requires at least: 4.4
Tested up to: 5.0
Requires PHP: 7.0
Multisite support: No
Stable tag: 1.1.0
License: GPLv3
License URI: http://www.gnu.org/licenses/gpl-3.0.html
Prefix: RVCTBS

Completely disables the category base from all URLs generated by WordPress so that there is no category slug displayed on archive permalinks, etc.

== Description ==

Completely disables the category base from all URLs generated by WordPress so that there is no category slug displayed on archive permalinks, etc.

* [**Join our FREE Facebook group for support**](https://www.facebook.com/groups/littlebizzy/)
* [**Worth a 5-star review? Thank you!**](https://wordpress.org/support/plugin/remove-category-base-littlebizzy/reviews/?rate=5#new-post)
* [Plugin Homepage](https://www.littlebizzy.com/plugins/remove-category-base)
* [Plugin GitHub](https://github.com/littlebizzy/remove-category-base)

#### Current Features ####

* changes post category URLs e.g. `/category/dogs/` to be simply `/dogs/`
* implements 301 redirects for proper SEO and usability
* does not affect "tags" base
* does not affect "parent" category base (e.g. `/animals/dogs/`)
* does not affect custom taxonomies
* does not affect product categories in WooCommerce
* works on category permalinks, category pagination, and category feeds
* works even if a custom category base is defined in settings

#### Compatibility ####

This plugin has been designed for use on [SlickStack](https://slickstack.io) web servers with PHP 7.2 and MySQL 5.7 to achieve best performance. All of our plugins are meant for single site WordPress installations only; for both performance and usability reasons, we highly recommend avoiding WordPress Multisite for the vast majority of projects.

Any of our WordPress plugins may also be loaded as "Must-Use" plugins by using our free [Autoloader](https://github.com/littlebizzy/autoloader) script in the `mu-plugins` directory.

#### Defined Constants ####

    /* Plugin Meta */
    define('DISABLE_NAG_NOTICES', true);

#### Technical Details ####

* Parent Plugin: [**SEO Genius**](https://www.littlebizzy.com/plugins/seo-genius)
* Disable Nag Notices: [Yes](https://codex.wordpress.org/Plugin_API/Action_Reference/admin_notices#Disable_Nag_Notices)
* Settings Page: No
* PHP Namespaces: No
* Object-Oriented Code: No
* Includes Media (images, icons, etc): No
* Includes CSS: No
* Database Storage: Yes
  * Transients: No
  * WP Options Table: Yes
  * Other Tables: No
  * Creates New Tables: No
* Database Queries: Backend Only (Options API)
* Must-Use Support: [Yes](https://github.com/littlebizzy/autoloader)
* Multisite Support: No
* Uninstalls Data: Yes

#### Special Thanks ####

[Alex Georgiou](https://www.alexgeorgiou.gr), [Automattic](https://automattic.com), [Brad Touesnard](https://bradt.ca), [Daniel Auener](http://www.danielauener.com), [Delicious Brains](https://deliciousbrains.com), [Greg Rickaby](https://gregrickaby.com), [Matt Mullenweg](https://ma.tt), [Mika Epstein](https://halfelf.org), [Mike Garrett](https://mikengarrett.com), [Samuel Wood](http://ottopress.com), [Scott Reilly](http://coffee2code.com), [Jan Dembowski](https://profiles.wordpress.org/jdembowski), [Jeff Starr](https://perishablepress.com), [Jeff Chandler](https://jeffc.me), [Jeff Matson](https://jeffmatson.net), [Jeremy Wagner](https://jeremywagner.me), [John James Jacoby](https://jjj.blog), [Leland Fiegel](https://leland.me), [Luke Cavanagh](https://github.com/lukecav), [Mike Jolley](https://mikejolley.com), [Pau Iglesias](https://pauiglesias.com), [Paul Irish](https://www.paulirish.com), [Rahul Bansal](https://profiles.wordpress.org/rahul286), [Roots](https://roots.io), [rtCamp](https://rtcamp.com), [Ryan Hellyer](https://geek.hellyer.kiwi), [WP Chat](https://wpchat.com), [WP Tavern](https://wptavern.com)

#### Disclaimer ####

We released this plugin in response to our managed hosting clients asking for better access to their server, and our primary goal will remain supporting that purpose. Although we are 100% open to fielding requests from the WordPress community, we kindly ask that you keep these conditions in mind, and refrain from slandering, threatening, or harassing our team members in order to get a feature added, or to otherwise get "free" support. The only place you should be contacting us is in our free [**Facebook group**](https://www.facebook.com/groups/littlebizzy/) which has been setup for this purpose, or via GitHub if you are an experienced developer. Thank you!

#### Our Philosophy ####

> "Decisions, not options." -- WordPress.org

> "Everything should be made as simple as possible, but no simpler." -- Albert Einstein

> "Write programs that do one thing and do it well... write programs to work together." -- Doug McIlroy

> "The innovation that this industry talks about so much is bullshit. Anybody can innovate... 99% of it is 'Get the work done.' The real work is in the details." -- Linus Torvalds

> "Software applications may follow the pattern of corporations. The desire to get more work done in a single application leads to bloated applications, just as the desire to avoid transaction costs leads to bloated bureaucracies. But bloated bureaucracies face competition from lean start-ups and eventually shed some of their bloat or die. Bloated software may face similar competition from leaner applications. There are some signs that consumers are starting to appreciate software and devices that do less and do it well." -- John D. Cook

#### Search Keywords ####

beautiful permalink, category to pages wud, custom permalinks, custom post type permalinks, fv top level categories, no category base (wpml), permalinks customizer, permalinks manager lite, remove category url, single category permalink, slightly troublesome permalink, woocommerce permalink manager, wp category permalink, wp no base permalink, wp remove category base

== Installation ==

1. Upload to `/wp-content/plugins/remove-category-base-littlebizzy`
2. Activate via WP Admin > Plugins
3. Test plugin is working:

After activating the plugin, purge all caches and then load one of the old category links that contains the `/category/` slug and it should be 301 redirected to a new "collapsed" URL that does not contain that slug.

== Frequently Asked Questions ==

= How can I change this plugin's settings? =

There is no settings page to maintain top performance and simplicity.

= Why is this plugin better than similar plugins? =

It uses a combination of techniques from other previous similar plugins. Also fixes a behaviour that does not worked well in the previous plugins and now is flushing properly the rewrite rules when the plugin is deactivated, so no need to regenerate the permalinks manually.

Also implements the compatibility with the SitePress plugin (WPML) at the moment of retrieve the current categories, among other technical improvements.

= I have a suggestion, how can I let you know? =

Please avoid leaving negative reviews in order to get a feature implemented. Instead, join our free Facebook group.

== Changelog ==

= 1.1.0 =
* tested with WP 5.0

= 1.0.6 =
* updated plugin meta

= 1.0.5 =
* partial transition to PHP namespaces
* optimized plugin code
* updated recommended plugins
* updated plugin meta

= 1.0.4 =
* added warning for Multisite installations
* updated recommended plugins

= 1.0.3 =
* better support for `DISABLE_NAG_NOTICES`

= 1.0.2 =
* tested with WP 4.9
* partial support for `DISABLE_NAG_NOTICES`
* updated plugin meta

= 1.0.1 =
* added recommended plugins notice
* added rating request notice
* updated plugin meta

= 1.0.0 =
* initial release
