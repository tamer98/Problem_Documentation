# Problems_Documentation
## Java Script
- writing ejs in a script is giving me the error 'Expression expected'<br/>

Problem : <br/>
```
<script> const post = <%- JSON.stringify(post) %> </script>
```

Solusion : <br/>
1)Change the global delimiters of EJS.<br/>
```
const ejs = require("ejs");

ejs.delimiter = '/';
ejs.openDelimiter = '[';
ejs.closeDelimiter = ']';
```

Update your script :
```
<script>
const post= [/- JSON.stringify(post) /];
</script>
```

2)Add this property to settings.json in VSCode :
```
"html.validate.scripts": false
```

By this steps : 

1. find html in bottom right
2. then find configure HTML language
3. and add line to end of json file

## Python

## MongoDB

## HTML

## Java

## C

## C++




