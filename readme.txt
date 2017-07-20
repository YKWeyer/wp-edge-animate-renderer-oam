=== WP Edge Animate OAM Renderer ===
Contributors: Thomas Vial <thomas.vial@ekino.com>, Vincent Composieux <vincent.composieux@ekino.com>, Damien Berseron <damien.berseron@ekino.com>
Donate link: http://www.ekino.com
Tags: adobe, oam, edge, animate, render
Requires at least: 3.0.1
Tested up to: 3.7
Stable tag: 1.1
License: MIT
License URI: http://opensource.org/licenses/MIT

Allows and renders OAM [Adobe Edge Animate](http://html.adobe.com/fr/edge/animate/) files in posts.
Contribute on http://www.github.com/ekino/wp-oam-renderer

== Description ==

* Allows upload for OAM files in Wordpress
* Unzips the `my_file.oam` in `my_file/` folder at the same location
* Provides automatic server-side iframe rendering for `<a href="http://site.com/wp-content/upload/2013/03/my_file.oam"></a>`
* Provides `[oam]` shortcode for manuel embed
* Deletes `my_file/` folder when `my_file.oam` is deleted from the library

== Installation ==

* Get the source from Github (https://github.com/ekino/wp-oam-renderer) or Wordpress SVN repository.
* Go to Admin > Plugins
* Activate wp-oam-renderer

== Usage ==

Simply insert your oam in your content from the media library using the "ATTACHMENT DISPLAY SETTINGS" name "Media File".
It will generate a link to the OAM file and will be rendered via an iframe.

= Getting size from animation =

`[oam id="28"]`

= Providing `width`, `height` will be calculated proportionaly =

`[oam id="28" width="960"]`

= Providing both `width` and `height` =

`[oam id="28" width="960" heigh="540"]`

== Parameters ==

* id *(mandatory)*
* width *(optional)*
* height *(optional)*

== Changelog ==

= 1.1 =
* Add display of OAM short code on media insert
* Fix code syntax to be compatible with PHP < 5.3
* Add display icon in "Insert media" post edition popin

= 1.0 =
* Initial version, code was refactored.
