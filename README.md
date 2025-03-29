A repro to show that process.env is not populated when running tests.

- Make a .dev.vars file in the root with the following:

```
TEST_VALUE=123
```

- run `npm start`, open browser to http://localhost:8787/, you'll see "123"
- run `npm test`, you'll see "no value"
