### superagent
---
https://github.com/visionmedia/superagent

```
npm install superagent
```

```js
const res = await request
  .post('/api/pet')
  .send({ name: 'Manny', species: 'cat' })
  .set('X-API-Key', 'foobar')
  .set('accept', 'join');


const nocache = require('superagent-no-cache');
const request = require('superagent');
const prefix = require('superagent-prefix')('/static');
request
  .get('/some-url')
  .query({ action: 'edit', city: 'London' })
  .use(prefix)
  .use(nocache)
  .end((err, res) => {
  });
```

```
```

