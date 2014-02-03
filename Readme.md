## Background
This library is heavily inspired by the [express-mongoose](https://github.com/LearnBoost/express-mongoose). It's offer the same features as express-mongoose but for the sequelize.

Methods which now support `Promises`:

   - `res.render`
   - `res.send`
   - `res.redirect`

Methods which now support `Queries`:

   - `res.render`
   - `res.send`

## Installation

    $ npm install express-sequelize

### Use

Include `express-sequelize` in your project, which performs the necessary bindings between `express` and `sequelize`.

```js
require('express-sequelize') // thats it!
```

### Example

```js
app.get('/user/:userId', function (req, res) {
  res.render('user', {
     user: User.find(req.params['userId'])
  });
});
```

## License

The MIT License (MIT)

Copyright (c) 2014 Zihua Li

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.