# How to get long parameters in Express.js

To get the path like this `/user/:id/abc.com`, we'll do like this:

1. 1st way: use `app.get('/user/*?')` ==> Got `:id/abc.com` via `req.params[0]`
2. 2nd way: `app.get('/user/:id*?')` ==> `req.params.id` => `:id`, `req.params[0]` => `/abc.com`