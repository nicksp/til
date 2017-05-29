# npm secrets

## Shorthand list

```sh
npm install pkg == npm i pkg
npm i --save pkg == npm i -S pkg
npm i --save-dev pkg == npm i -D pkg
npm test == npm t
```

### Quick package initialization

```sh
npm init -y
```

### List available scripts

```sh
npm run
```

### List installed packages


#### Local packages

```sh
npm ls --depth 0
```

#### Global packages

```sh
npm ls -g --depth 0
```

### Running locally-installed executables

```sh
./node_modules/.bin/<command>
```

### Open current package on npmjs.com

```sh
npm docs
```

### Bumping package’s version

```sh
npm version major/minor/patch
```
