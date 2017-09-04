## MediaWiki Info Extension

Adds a Info `&action=info` link tab of regular articles to your MediaWiki Skin allowing quick displaying of page informations.

### Installation

Download and upload the zip file to `/extensions` and extract. Rename directory folder `/Info-#-#-#` to `/Info` and add the following to `LocalSettings.php` to enable this extension.

`require_once "$IP/extensions/Info/Info.php";`

Control the ability by user group to info content. eg `['*']` would allow anyone, `['user']` allows only users or `['sysop']` would only allow sysops.

`$wgGroupPermissions['{a user group}']['info'] = true; # allow viewing Info for a specific user group

See https://www.mediawiki.org/wiki/Extension:Info for more information about displaying a page's informations.
