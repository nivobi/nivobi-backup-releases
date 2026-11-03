# Changelog

## 0.9.0
- Renamed to Nivobi Backup & Migration (folder nivobi-backup). Backups are now .nivobi files and the WP-CLI command is wp nivobi. Builds named WPBK (0.8.0 and older) cannot update to this one: delete the old plugin and install this zip.
- Prepared for wordpress.org: Plugin Check clean, readme.txt, a build without the GitHub updater.

## 0.8.0
- Restore onto an empty server: download wpbk-installer.php from Restore & move, upload it with a backup to the new host's empty folder, open it and follow the steps. It installs WordPress (checked file by file against wordpress.org), writes wp-config.php, installs WPBK, restores the backup and removes itself.
- Unlocking the installer needs proof of file access, like the emergency page; it refuses a folder that already holds a site.

## 0.7.0
Emergency restore page (on by default, can be turned off in Settings): when WordPress shows a white screen or you cannot log in, open wp-content/plugins/wpbk/emergency.php. Unlock it by creating the file it names in wp-content over FTP, then switch plugins off, move must-use plugins and drop-ins aside, undo an update or restore a backup.
Settings shows the page's address; the Overview shows when it was last used.

## 0.6.0
Backup before updates (off by default, turn on under Settings): before a plugin or theme update, WPBK saves its old folder, and the database when it fits in a few seconds. Never blocks an update.
"Undo this update" on the Backups page puts the old version back, optionally with the database.
Pre-update backups are kept 7 days or 5 update runs (adjustable) and never count as the site's backup.

## 0.5.0
- Partial restore: restore only the database, chosen plugins or themes, media or the rest of wp-content from a backup (Restore page > Choose parts, or wp wpbk import --parts / --plugins / --themes)
- A partial media restore puts back files from the backup and keeps uploads made since then
- The safety snapshot and rollback of a partial restore cover only what it replaces

## 0.4.4
- Updates now show up even when the site cannot reach wordpress.org at that moment.

## 0.4.3
- New versions now show up as soon as you open Dashboard → Updates, instead of up to 12 hours later.

## 0.4.2
- The Plugins screen now shows the plugin is by nivobi, with a link to nivobi.com.

## 0.4.1
- The backup sizes in the Overview list now line up in one column.

## 0.4.0
- Updates now arrive under Plugins: no more uploading zips by hand.
- New admin look: an app window with a dark teal sidebar.
- New dashboard with Overview, Backups, Restore & move, Storage and Settings pages.
- Needs WordPress 6.6 or newer.
