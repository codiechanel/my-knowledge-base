By default, string replace only replaces the first occurrence. If you want to replace all, you need to use regex with the global parameter.
```javascript
var str = 'hello i am'
str.replace(new RegExp('hello', 'g'), 'great')
```



