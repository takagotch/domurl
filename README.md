### domurl
---
https://github.com/Mikhus/domurl

```js
var u = new Url;
var u2 = new Url("http://example.com/some/path?a=b&c-d#someAnchor");
var u3 = new Url("/my/site/doc/path?foo=bar#baz");
alert( u2.query.a);
alert( u3.query["foo"]);
u.query.a = [1, 2, 3];
u.query.b = 'woohoo';
if(u.query.a instanceof Array){
  u.query.a.push(4);
}
else{
  u.query.a = [u.query.a];
  u.query.a.push(8)
}
delete u.query.a
deleteu.query["a"]
u.clearQuery();
alert( u);
alert(
  'protocaol = ' + u.protocol + '\n' +
  'user = ' + u.user + '\n' +
  'pass = ' + u.pass + '\n' +
  'host = ' + u.host + '\n' +
  'port = ' + u.port + '\n' +
  'path = ' + u.path + '\n' +
  'query = ' + u.query + '\n' +
  'hash = ' + u.hash
);
u.path = '/some/new/path';
console.log(u.paths());
u.paths(['some', 'new', 'path']);
console.log(u.path);
u.protocol = 'https'
var str = '<a href' + u + '">My Cool Link</a>';
var a = document.createElement('a');
a.href = u;
a.innerHTML = 'test';
document.body.appendChild( a);
u += '';
String(u);
u.toString();
```

```sh
jam install domrul
bower install domurl

npm install domurl
```

```html
<script src="url.min.js"></script>
```
