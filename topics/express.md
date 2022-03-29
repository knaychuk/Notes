# Create a Server

```javascript
const express = require('express');
const app = express();

app.listen(3000, () => {});

```

# Response

```javascript
app.get('./PathToListenTo', (req, res) => {});

//sets status code & content-type automatically
```