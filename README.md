# yarn-vue-eslint
Sample code for this issue: https://stackoverflow.com/questions/59614362/why-does-vue-cli-service-build-fail-after-creating-a-new-eslint-plugin-with-e when following this eslint custom rule tutorial: https://blog.webiny.com/create-custom-eslint-rules-in-2-minutes-e3d41cb6a9a0

# Running `yarn build` (`vue-cli-service build`) gives the error:
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

# This project was created by:
`vue create eslint-test-project` (default babel and eslint preset)

`cd eslint-test-project`

`vue add eslint` (choose airbnb and lint on save)

create `/eslint/` and its files as per steps 1 to 3 of [this tutorial](https://blog.webiny.com/create-custom-eslint-rules-in-2-minutes-e3d41cb6a9a0)

`yarn add --dev file:./eslint` (step 4)

create `eslintrc.js` as per step 5 of [this tutorial](https://blog.webiny.com/create-custom-eslint-rules-in-2-minutes-e3d41cb6a9a0), but removing the mentioned non-custom rule (flowtype)

`yarn build`
