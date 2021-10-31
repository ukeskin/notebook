# Express

#### Import express
```js
const express = require('express')
const app = express()
```
###  Respond with "hello world" when a GET request is made to the homepage
```js
app.get('/', function (req, res) {
  res.send('hello world')
})
```

### To define routes with route parameters
```js
app.get('/users/:userId/books/:bookId', function (req, res) {
  res.send(req.params)
})
```
