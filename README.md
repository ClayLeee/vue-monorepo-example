# VueJS + Lerna monorepo project sample

This is repository supports the content of the article: [VueJS - Building a basic Monorepo project](https://dev.to/vcpablo/vuejs-building-a-monorepo-using-lerna-1h1c)

## Project setup (installs all root dependencies and all dependencies of all inner modules)
```
yarn refresh
```

### Compiles and hot-reloads `addition` module for development
```
yarn dev:addition
```

### Compiles and minifies `addition` module for production
```
yarn build:addition
```

### Tests `addition` module
```
yarn test:addition
```
### Compiles and hot-reloads `multiplication` module for development
```
yarn dev:multiplication
```

### Compiles and minifies `multiplication` module for production
```
yarn build:multiplication
```

### Tests `multiplication` module
```
yarn test:multiplication
```

### Lints and fixes all module files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
