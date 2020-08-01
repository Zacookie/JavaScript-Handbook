### Debugging:
For when you can't track that one pesky error down:
• Node.js: https://nodejs.org/en/docs/guides/debugging-getting-started/
• VSCode: https://code.visualstudio.com/docs/nodejs/nodejs-debugging
• Lint (syntax errors and code consistency): https://discordjs.guide/preparations/setting-up-a-linter.html
• MDN list of common errors: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors
• Guide on common errors and how to deal with them: https://discordjs.guide/popular-topics/errors
• Discord.js: attach the following two listeners to your Client instance (outside of any other listener scopes)

```js
client.on("debug", console.log)
      .on("warn", console.log)
```

*Note: if you initialize your Client as botor other identifiers you need to use these instead of client.*