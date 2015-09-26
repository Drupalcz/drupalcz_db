# Drupal.cz Database 
Helper repo to share scrubbed database dump of D6 drupal.cz.

* DB must be always scrubbed by using https://github.com/Drupalcz/drupalcz/blob/develop/scrub.sql
* Commit messages must contain SHA1 ref to the version of scrub.sql used to scrub DB.
* Commit messages must contain database snapshot date.

## Contents
* `dcz_scrubbed.sql` - Fullsize DB without caches and sensitive data replaced with placeholders.
* `dcz_scrubbed_slim.sql` - Light weight version of DB for quicker testing. Sensitive data replaced with placeholders.

## Tools
* Scripts to generate these files are here: https://github.com/Drupalcz/drupalcz
* Source database to run these scripts on is private. Doh.
* `dcz_scrubbed.sql` uses `scrub.sql`
* `dcz_scrubbed_slim.sql` uses `scrub.sql` and `slim.sql`
