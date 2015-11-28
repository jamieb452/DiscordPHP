# User

The user class is the base for any user that exists in any guild you are apart of.

# Attributes

- `id` The identifier of the user.
- `username` The username of the user.
- `avatar` The avater URL of the user.
- `discriminator` Distinguishes between two users with the same username.

- `avatar_id` The avatar ID of the user.

# Functions

## `User@sendMessage`

Sends a message to the user. Returns a [`Message`](parts/message.md).

- `$message`	`string` 	The message to send to the user.
- `$tts`		`boolean`	If the message is sent as talk-to-speech.	Default `false`.

```php
$user->sendMessage('Hello world!', false);
```

## `User@broadcastTyping`

Broadcasts that you are typing to the user.

```php
$user->broadcastTyping();
```