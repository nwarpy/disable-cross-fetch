# Usage

Used to disable cross-fetch in environments where fetch works but cross-fetch doesn't (like Cloudflare Workers).

```
npm i disable-cross-fetch
```


Add the following to your package.json

```
{
  "overrides": {
    "cross-fetch": "npm:disable-cross-fetch"
  }
}
```

Due to a bug that seems to persist even in npm v8.19.4, you might need to delete node_modules and package-lock.json and install everything again.

https://github.com/npm/cli/issues/4232