# Create a Server

```javascript
const http = require('http');

http.createServer((req, res) => {});

server.listen(3000, 'localhost', () => {});
 ```
# Setting the Content Type

```javascript
res.setHeader('Content-Type', 'text/html'); //put this in create server function
                                            //uses html as an example

```
# Using the File System 

```javascript
const fs = require('fs');
```

#### Reading Files

```javascript
fs.readFile('./PathToFile', (err, data) => {
  if(err) {
    console.log(err);   //if error, do something
  }
  console.log(data);   //use data.toString() to turn buffer into text
});
```

#### Writing Files

```javascript
fs.writeFile('./PathToFile', 'content to write', () => {}); 
```

#### Other Basic Methods

```javascript
//Make Directory
fs.mkdir('./PathToDir', (err) => {});

//Remove Directory
fs.rmdir('./PathToDir', (err) => {});

//Delete File
fs.unlink('./PathToFile', (err) => {});
```

# Streams & Buffers
 