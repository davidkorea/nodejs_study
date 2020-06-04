
# http

nodejs自带http模块

- `server.js`
```javascript
'use strict'

var http = require('http')

var app = http.createServer((req, res)=>{
    res.writeHead(200,{'Content-Type':'text/plain'})
    res.end('hello nodejs world')
}).listen(80,'0.0.0.0')
```

1. `node server.js`
2. `forever start server.js`, run background forever
    - `npm install forever -g`
