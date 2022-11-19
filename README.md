# wp-config.php

## Environments

### Local Dev Environment

```php
define( 'WP_DEBUG', true );
define( 'WP_DEBUG_LOG', true );
define( 'WP_DEBUG_DISPLAY', true ); 

define( 'CONCATENATE_SCRIPTS', false );
```

## Disable External API Call

```
define( 'WP_HTTP_BLOCK_EXTERNAL', TRUE );


// Allow some hosts
define( 'WP_ACCESSIBLE_HOSTS', 'wordpress.org', 'api.wordpress.org' );
```

## Disable post revisions

```php
define( 'WP_POST_REVISIONS', false );
```

### Production Environment

**Disable cron jobs**

```php
define( 'DISABLE_WP_CRON', true );
```

**Set memory limit**

```php
define( 'WP_MEMORY_LIMIT', '96M' );
define( 'WP_MAX_MEMORY_LIMIT', '128M' );
``

**Limit trash auto clean**

```php
define( 'EMPTY_TRASH_DAYS', 3 ); // days
``

**Disable all automatic updates**

```php
 # Disable all core updates:
 define( 'WP_AUTO_UPDATE_CORE', false );
 
 # Enable all core updates, including minor and major:
 define( 'WP_AUTO_UPDATE_CORE', true );
 
 # Enable core updates for minor releases (default):
 define( 'WP_AUTO_UPDATE_CORE', 'minor' );
```

**Disable theme and plugin editing**

```php
define( 'DISALLOW_FILE_EDIT', true );
define( 'DISALLOW_FILE_MODS', true );
```

### WP Admin Recovery Mode

**Disable admin recovery mode**

```php
define( 'WP_DISABLE_FATAL_ERROR_HANDLER', true );
```

**Replace recovery email notification**

```php
define( 'RECOVERY_MODE_EMAIL', 'dev@codetot.com' );
```
