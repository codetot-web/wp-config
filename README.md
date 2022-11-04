# wp-config.php

## Environments

### Local Dev Environment

```php
define( 'WP_DEBUG', true );
define( 'WP_DEBUG_LOG', true );
```

### Production Environment

**Disable all automatic updates**

```php
define( 'AUTOMATIC_UPDATER_DISABLED', true );
```

**Disable only core updates**

```php
define( 'WP_AUTO_UPDATE_CORE', false );
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
