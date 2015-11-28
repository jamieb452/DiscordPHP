# Welcome

Welcome to the DiscordPHP documentation! This is still a work in progress and will improve once the API has been finished.

To start off, view the `Install` section below.

# Install

To install DiscordPHP you need to be using [Composer](https://getcomposer.org). Composer is a free and easy package dependency manager.

Once you have Composer installed into your project, type the following into your console:

```
$ composer require team-reflex/discord-php
```

If you haven't used Composer before, now is the time you would include the Composer autoload file:

```php
<?php

include 'vendor/autoload.php';
```

# First Use

Once you have DiscordPHP installed, the first thing to do is authenticate with the Discord servers:

```php
<?php

use Discord\Discord;

$discord = new Discord(':email-address', ':password');
```

If you don't want to have your Email or Password in plain text, you can use a Composer package called `PhpDotEnv` or you can find you Discord token and enter it as a third parameter like so:

```php
$discord = new Discord(null, null, ':token');
```

From here you can interact with the `Client` class, which has more information on other pages.

# `Discord` class usage

## Logging out

To log out of Discord, use the following function.

```php
$discord = new Discord();
$discord->logout();
```

## Accepting invites

You can accept instant invites by doing the following.

```php
$discord = new Discord();
$discord->acceptInvite(':code');
```

**Note:** Using the full URL will not work. You need to only enter in the actual code.