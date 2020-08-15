# node-typescript-cheatsheet

Cheatsheets for experienced Node.js developers getting started with TypeScript

## Helpful tools

- https://ts-engine.dev/
- https://github.com/gcanti/io-ts flowing runtime tests down and doing validation in runtime 
  - podcast discussion https://fullstackradio.com/episodes/144
- attaching properties on to `req` in Express https://twitter.com/mjackson/status/1294384799231012864?s=20


## Tip 1

`tsconfig.json`:

```json
{
  "compilerOptions": {
    "target": "es2015",
    "module: "commonjs"
  }
}
```

## Tip 2

shipping typescript sourcemaps from a node server: http://npm.im/source-map-support

## Tip 3

Instead of

```bash
nodemon --exec ts-node src/index.ts
```

do:

```bash
tsc --watch
nodemon dist/src/index.js
```

https://twitter.com/benawad/status/1211700652549779456
