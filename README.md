
# Discord Rich Presence

A simple wrapper around [discord-rpc](https://npmjs.org/discord-rpc)

### Example

```javascript
const client = require('discord-rich-presence')('Bot_ID');

client.updatePresence({
  state: 'Test',
  details: 'Test',
  startTimestamp: Date.now(),
  endTimestamp: Date.now() + 1337,
  largeImageKey: 'snek_large',
  smallImageKey: 'snek_small',
  instance: true,
});
```

In browser you can import/require it as `discord-rich-presence/browser`.
However, it should be noted that currently using rich presence in browser is
a feature whitelisted by Discord, and you will most likely be unable to use it.
