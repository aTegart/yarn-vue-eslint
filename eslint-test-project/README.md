# eslint-test-project

## Running `yarn build` (`vue-cli-service build`) gives the error:
```
Module build failed (from ./node_modules/thread-loader/dist/cjs.js):
Thread Loader (Worker 0)
eslint.CLIEngine is not a constructor
    at PoolWorker.fromErrorObj (/Users/anna/projects/yarn-vue-eslint/eslint-test-project/node_modules/thread-loader/dist/WorkerPool.js:262:12)
    at /Users/anna/projects/yarn-vue-eslint/eslint-test-project/node_modules/thread-loader/dist/WorkerPool.js:204:29
    at mapSeries (/Users/anna/projects/yarn-vue-eslint/eslint-test-project/node_modules/neo-async/async.js:3625:14)
    at PoolWorker.onWorkerMessage (/Users/anna/projects/yarn-vue-eslint/eslint-test-project/node_modules/thread-loader/dist/WorkerPool.js:170:35)
    at readBuffer (/Users/anna/projects/yarn-vue-eslint/eslint-test-project/node_modules/thread-loader/dist/WorkerPool.js:152:14)
    at Object.module.exports (/Users/anna/projects/yarn-vue-eslint/eslint-test-project/node_modules/eslint-loader/index.js:223:27)
```
----------------------------------------------------------------
## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
