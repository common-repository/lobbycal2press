=== Plugin Name ===
Contributors: lobbycalDec
Donate link: https://www.transparency.org/donate/
Tags: calendar, meeting management, office, relations
Requires at least: 4.0
Tested up to: 4.9.7
Stable tag: trunk
License: CC0 1.0 Universal
License URI: https://creativecommons.org/publicdomain/zero/1.0/

 Show meetings managed on a lobbycal server

== Description ==

This plugin displays meetings published on a lobbycal server in a table on any page in your wordpress installation.
You need to know your lobbycal URL if you want to display your meetings with the plugin. 


== Installation ==

1. Upload the plugin files to the `/wp-content/plugins/plugin-name` directory, or install the plugin through the WordPress plugins screen directly.
1. Activate the plugin through the 'Plugins' screen in WordPress
1. Use the Settings->lobbycal2press screen to configure the plugin
1. To use the plugin in wordpress 
1. in your wordpress installation, adapt the URL to your lobbycal server account at Settings > Lobbycal2press
1. place the table html fragment from https://plugins.svn.wordpress.org/lobbycal2press/trunk/readme.txt in a page, where you would like the calendar to appear

`<table id="lobbycal" aria-describedby="lobbycal_info">    <thead>        <tr>            <th>Date</th>            <th>End</th>            <th>FirstName</th>            <th>LastName</th>            <th>Partners</th>            <th>Title</th>            <th>Tags</th>        </tr>    </thead></table>`




== Frequently Asked Questions ==

= I do not have a lobbycal server =

Get yours here: `https://github.com/TransparencyInternationalEU/lobbycal`

= Can I see it in production somewhere =

Lobbycal is used here https://lobbycal.greens-efa-service.eu/all

= I would like to show meetings of all users=

After registration you should have received an email with your personal API URL.

It should be similar to 

`http://our-lobbycal-server.org/api/meetings/dt/100`

To display all meetings published by that lobbycal server instance, simply remove the id at the end of the URL

`http://our-lobbycal-server.org/api/meetings/dt`

For wordpress, this is done at the plugins settings page /wp-admin/options-general.php?page=lobbycal2press
 
= I would like to show meetings of selected users=

To display meetings of selected users, simply add ids of these users at the end of the URL, separated by comma.

`http://our-lobbycal-server.org/api/meetings/dt/42,23`

For wordpress, this is done at the plugins settings page /wp-admin/options-general.php?page=lobbycal2press 

= I don't want line breaks in the partner / tag column = 
OK. Go to the plugin editor in your wordpress installation and edit lobbycal2press.js. 
Scroll down to 'function partner'. 
Remove '<br/>' .
Save and refresh. 

== Changelog ==

n/a