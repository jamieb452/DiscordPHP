# Guild

The guild is Discord's name for Server.

# Attributes

- `id` The identifier for the Guild.
- `name` The name for the Guild.
- `icon` The icon for the Guild.
- `region` The region the Guild's voice server is hosted in.
- `owner` The owner of the Guild.
- `joined_at` A `DateTime` instance of when the current user joined the guild.
- `afk_channel_id` The channel ID of the AFK voice channel.
- `afk_timeout` How long you timeout of the AFK voice channel.
- `embed_enabled` If the Discord embed is enabled on this Guild.
- `embed_channel_id` The ID of the channel that is embedded.

- `roles` An array of [`Roles`](roles.md) that belong to the Guild.
- `channels` An array of [`Channels`](../channels/channel.md) that belong to the Guild.
- `members` An array of [`Members`](../user/member.md) that belong to the Guild.
- `bans` An array of [`Bans`](ban.md) that belong to the Guild.
- `owner_id` The owner ID of the guild.

# Constants

- `REGION_DEFAULT` The default region for new servers, currently `REGION_US_WEST`.
- `REGION_US_WEST` West Coast, United States.
- `REGION_US_EAST` East Coast, United States.
- `REGION_SINGAPORE` Singapore.
- `REGION_LONDON` London, United Kingdom.
- `REGION_SYDNEY` Sydney, Australia.
- `REGION_AMSTERDAM` Amsterdam, Netherlands

# Functions

## `Guild@validateRegion`

Validates the set region and returns it if it is valid, otherwise returns the default.

```php
$guild->validateRegion();
```