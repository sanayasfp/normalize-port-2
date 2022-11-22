# normalize-port

A handy function that normalizes a port into a number, string, or false.

## install

`npm install --save normalize-port-2`

## usage

```javascript
const http = require("http");
const normalizePort = require("normalize-port-2");

const port = normalizePort(process.env.PORT || "8080");

const server = http.createServer(listenerOrApp).listen(port, () => {
    console.log(`Server running: http://127.0.0.1:${port}.`);
});
```

```typescript
import http from "http";
import normalizePort from "normalize-port-2";

const port = normalizePort(process.env.PORT || "8080");

const server = http.createServer(listenerOrApp).listen(port, () => {
    console.log(`Server running: http://127.0.0.1:${port}.`);
});
```

## credit

I just pulled this little function out of the
[normalize-port](https://www.npmjs.com/package/normalize-port) package.
