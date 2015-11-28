# Member

The member class is a link between a [`User`](user.md) and a [`Guild`](guild.md).

# Attributes

- `user` The [`User`](user.md) instance of the member.
- `guild` The [`Guild`](../guilds/guild.md) instance of the member.
- `deaf` The users state of deaf.
- `mute` The users state of mute.
- `joined_at` A `DateTime` instance of when the `User` joined the `Guild`.
- `guild_id` The ID of the `Guild` the member belongs to.

# Functions

## `Member@kick`

Kicks the member from the Guild. Alias for `Part@delete`.

```php
$member->kick();
```