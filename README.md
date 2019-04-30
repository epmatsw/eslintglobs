# Instructions

`npm test` demonstrates https://github.com/eslint/eslint/issues/11558. `src/a.js` should not have `no-var` applied because the override should disable it. `src/b.js` should be ignored.

`npm run control` runs a control test where it uses the same configuration but in a different location. I would expect the behavior to be the same, but in this case we get the expected behavior where `src/a.js` is correctly not flagged.