=== WOW Server Status Widget ===
Contributors: ycfreeman
Donate Link: http://ycfreeman.com
Tags: WOW, Warcraft, World of Warcraft, Realm, Server, Status, widget, wow
Requires at least: 2.8
Tested up to: 4.5
Stable tag: 1.0.13

Easily add WOW Server Status 4.1 badge to your wordpress site by just a few clicks.

== Description ==

This is a simple widget that displays WOW Server Status 4.1 badge, without having to upload the script with ftp and write an img tag to run it.
-- realms with non-english names may also work, but not in 'full' mode as the font used doesn't have those characters

The original script [can be found here](http://53x11.com/blog/2005/04/21/WoW-Server-Status-41.10), which is not my work 
1.0.6: patched to use official JSON feed (finally :p), php 5.2+ recommended (for native json_decode() support), fallback JSON.php for earlier versions is included as well.

** If you find your widget broken after a wordpress core update, please try to re-save your widget settings.

If you managed to find bugs or want to correct some of my codes, please don't hesitate to post on forum:)

* [Plugin Page](https://wordpress.org/plugins/wow-server-status-widget/)
* [Demo](http://ycfreeman.com/wssdemo/)
* [Full Plugin Description](http://ycfreeman.com/blog/2010/06/wow-server-status-wordpress-widget-10/)
* [Issue Tracker](https://github.com/ycfreeman/wow-server-status-widget/issues)
* [Source Code](https://github.com/ycfreeman/wow-server-status-widget)

== Installation ==
1. Unpack and Upload all files to the `/wp-content/plugins/wow-server-status-widget` directory
1. Add your Battle.net API key in Settings
1. Activate the plugin through the **Plugins** menu in WordPress
1. Drag **WOW Server Status Widget** to your sidebar
1. Enter details and done!

== Frequently Asked Questions ==
The badge script is not my work, I just make it easy to drag and drop in wordpress.
It should be able to run properly on most servers, but if there is a problem
please visit [the author's site](http://53x11.com/blog/2005/04/21/WoW-Server-Status-41.10) and look for solutions there.

= It says "No Status Source", what's wrong? =
Make sure you have got a correct Battle.net API key [get one here](https://dev.battle.net/), also check the realm name and region carefully, it won't work if you've typed it wrong.
If [official realm status page for US](http://us.battle.net/wow/en/status) or [official realm status page for EU](http://eu.battle.net/wow/en/status) is working fine, this badge should be working fine, in some rare cases like when Blizzard is upgrading their server hardware or something, the realm page just breaks and this badge will also break.

= It doesn't reflect the actual realm status correctly, what's wrong? =
See above. Also, cache time of this badge is set to 5 minutes, so it may not reflect immediately if the server status has just changed within 5 minutes.


== Screenshots ==
1. Here is how it looks

== Changelog ==

= 1.0.13=
* add widget settings page for API key settings

= 1.0.8 =
* update bug report icon and url

= 1.0.7 =
* fixed a mis-uploaded file

= 1.0.6 =
* patched to use official JSON feed

= 1.0.5 =
* fixed bug of space becomes %20 in the new wow_ss.php, thanks Mike

= 1.0.4 =
* since official realm status xml is not there anymore, I've modified the original wow server status badge to use [Axho's WoW Feeds](http://wowfeeds.wipeitau.com/)... at least for now, feel free to extract the modified badge php for your own use.

= 1.0.3 =
* take 2, fixed the apostrophe realm not showing bug in original wow_ss.php, aparently the original script has 3 places doing the same thing, so I merged them to one, and encode it correctly to ANSI
it should be fine now if your keyboard is US keyboard, that renders apostrophe as &#039;, sorry for having it not working for so long

= 1.0.2 =
* fixed the apostrophe realm not showing bug in original wow_ss.php, thanks Nullinger

= 1.0.1 =
* better plugin path handling, added bug report icon, updated license wordings

= 1.0 =
* First released version

== Upgrade Notice ==
