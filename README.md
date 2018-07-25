# Instructions

Clone project: `git clone git@github.com:ajbogh/import_loop_flow_bug.git`

Install packages: `npm install`

Run test: `npm run test`

When Flowtype fails you will notice an error that looks like this:

```
> jest

 FAIL  __tests__/layout-engine.test.js
  ● Test suite failed to run

    TypeError: Super expression must either be null or a function, not undefined



      at _inherits (src/flowtype/none.js:14:113)
      at src/flowtype/none.js:19:3
      at Object.<anonymous> (src/flowtype/none.js:28:2)
      at Object.<anonymous> (src/flowtype/layout-engine-config.js:2:1)
      at Object.<anonymous> (src/flowtype/graph-view.js:2:1)
      at Object.<anonymous> (src/flowtype/layout-engine.js:2:1)
      at Object.<anonymous> (__tests__/layout-engine.test.js:1:1)

 PASS  __tests__/layout-engine.test.ts

Test Suites: 1 failed, 1 passed, 2 total
Tests:       1 passed, 1 total
```

The error above indicates that the Flowtype test failed while the Typescript test succeeded.
