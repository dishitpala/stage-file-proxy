# Stage File Proxy

Mirror (or header to) uploaded files from a remote production site on your local development copy. Saves the trouble of downloading a giant uploads directory without sacrificing the images that accompany content.

## Configuration
Define below constants in your wp-config.php file to configure Stage File Proxy plugin features.

```php
// Define proxy url to fetch media from.
define( 'STAGE_FILE_PROXY_URL', 'https://global.videojet.com/wp-content/uploads/' );

/**
 * Define mode to mirror the media.
 *
 * Default
 * - 'header' Header mode is used to fetch the media from STAGE_FILE_PROXY_URL and does not store any media in local
 *
 * Options
 * - 'header' Header mode is used to fetch the media from STAGE_FILE_PROXY_URL and does not store any media in local
 * - 'download' mode is used to fetch the media from STAGE_FILE_PROXY_URL and store media in local
 */
define( 'STAGE_FILE_PROXY_MODE', 'header' );
```