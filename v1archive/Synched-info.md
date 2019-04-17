# Information we Synch

## credits (not stored)
- WordPress version
- Locale

## core/version-check (all stored, except for those marked)
- Site URL
- Site IP address
- WordPress version
- PHP version
- MySQL version
- Locale
- Number of sites (i.e., on a multisite install) (not stored)
- Number of users (not stored)
- Whether multisite is enabled or not
- On Multisite installs, the URL of the parent blog (i.e., the parent blog of pento.blog is wordpress.com)
- Initial DB version (corresponds with the version of WordPress that was initially installed for this site)
- Report data on whether a site updated successfully or not

## plugins/update-check
- Site URL (stored)
- A list of all plugins installed (stored)
- A list of all plugin translation files installed
- A list of all locales enabled on the site

## themes/update-check
- Site URL (stored)
- A list of all themes installed (stored)
- A list of all theme translation files installed
- A list of all locales enabled on the site

## events: Information is hashed to create a cache key (i.e., so two people searching for “nyc” will get the same result). The hash can’t be reversed.
- User’s partially anonymised IP address (e.g., 1.2.3.0, the last digit will always be 0)
- Browser timezone
- User entered location

## core/importers (not stored)
- WordPress version
- Locale

## translations (not stored)
- WordPress version
- Locale
- Plugin/theme version
- Plugin/theme slug

## themes/info (not stored)
- User entered search data

## plugins/info (not stored)
- List of installed plugins

## core/checksums (not stored)
- WordPress version
- Locale

## core/browse-happy (1 in 25 requests stored)
- WordPress version
- Site URL
- Browser useragent
