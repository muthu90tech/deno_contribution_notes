# comparing deno to node when runtime starts and executes scripts

consider a script like
```
console.log('test')
```

NodeJS
`lib/internal/process/prepareExecution.js` which launches several IPC channel.

TODO: find deno side of things..