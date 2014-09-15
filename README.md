# express-defaultlocals

`npm install express-defaultlocals --save`

Similar to dynamicHelpers of express 2.0, but as a middleware for express 4.0.

Because it's done as a middleware, you can use it on a router rather than on app, e.g.:

```js
router.use(defaultLocals(function(req) {
  return {
    user: req.user
  }
}))
```
