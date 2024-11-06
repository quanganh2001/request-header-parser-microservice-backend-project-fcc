My solution:
```js
app.get('/api/whoami', function (req, res) {
  res.json({
    ipaddress: req.socket.remoteAddress,
    language: req.headers['accept-language'],
    software: req.headers['user-agent']
  });
});
```
