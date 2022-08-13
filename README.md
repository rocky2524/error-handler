# error handler


paste this code in index.js or your code file

```
process.on('unhandledRejection', (reason, p) => {
    console.log('ignore that log');
  });
  process.on("uncaughtException", (err, origin) => {
    console.log('ignore that log');
  })
  process.on('uncaughtExceptionMonitor', (err, origin) => {
    console.log('ignore that log');
  });
  process.on('beforeExit', (code) => {
    console.log('ignore that log');
  });
  process.on('exit', (code) => {
    console.log('ignore that log');
  });
  process.on('multipleResolves', (type, promise, reason) => {
    console.log('ignore that log');
  });
```
this prevents to stop bot automatically when its get error in console



