# comparing deno to node when runtime starts and executes scripts

consider a script like
```
console.log('test')
```

NodeJS
`lib/internal/process/prepareExecution.js` which launches several IPC channel.

Wrote a c.ts, in ext/node/polyfills/c/c.ts
which will dynamically load either child or primary based on a env var.

Have to next figure out the entrypoint in deno which preps execution environment.