# Changelog

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
