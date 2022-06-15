This repo demonstrates an issue with `eslint-plugin-import`,
`eslint-import-resolver-webpack`, and `socket.io-client`.

To reproduce this issue, clone this repository, then run the following commands:

```
npm install
npm run lint
```

Note the error "Unable to resolve path to module 'socket.io-client'" even though
`socket.io-client` is installed.

Note that the webpack build completes without error, indicating that webpack is
able to resolve `socket.io-client`.

```
npm run build
```
