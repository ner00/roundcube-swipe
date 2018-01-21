Roundcube Webmail Swipe
=======================
This plugin adds left/right/down swipe actions to entries in the the message
list on touch devices (tables/phones) with browsers that support touch events.

ATTENTION
---------
This is just a snapshot from the GIT repository and is **NOT A STABLE version
of Swipe**. It is Intended for use with the **GIT-master** version of
Roundcube and it may not be compatible with older versions. Stable versions of
Swipe are available from the [Roundcube plugin repository][rcplugrepo]
(for 1.4 and above) or the [releases section][releases] of the GitHub
repository.

License
-------
This plugin is released under the [GNU General Public License Version 3+][gpl].

Even if skins might contain some programming work, they are not considered
as a linked part of the plugin and therefore skins DO NOT fall under the
provisions of the GPL license. See the README file located in the core skins
folder for details on the skin license.

Install
-------
* Place this plugin folder into plugins directory of Roundcube
* Add swipe to $config['plugins'] in your Roundcube config

**NB:** When downloading the plugin from GitHub you will need to create a
directory called skin and place the files in there, ignoring the root
directory in the downloaded archive.

Supported skins
---------------
* Elastic

Configuration
-------------
To set the default actions add `$config['swipe_left']`, `$config['swipe_right']`
and `$config['swipe_down']` to your Roundcube config file. For example:
`$config['swipe_left'] = 'delete';`. Users can configure the actions, overriding
the defaults, from the List options menu.

Supported actions
-----------------
The following actions are available for left/right swipe:

* `archive` - Archive the message (Requires the Roundcube Archive plugin)
* `delete` - Delete the message
* `flagged` - Mark the message as flagged/unflagged
* `forward` - Forward the message
* `move` - Move the message to a chosen folder
* `read` - Mark the message as read/unread
* `reply` - Reply to the message
* `replyall` - Reply all to the message
* `select` - Select/deselect the message
* `none` - Swipe disabled

The following actions are available for down swipe:

* `checkmail` - Check for new messages in the current folder
* `none` - Swipe disabled

[rcplugrepo]: https://plugins.roundcube.net/packages/johndoh/swipe
[releases]: https://github.com/johndoh/roundcube-swipe/releases
[gpl]: https://www.gnu.org/licenses/gpl.html