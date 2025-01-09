# Internal packages

- **Node.js provides you some `packages` in the node.js. Some common ones include**
1. fs - Filesystem
2. path - Path related functions
3. http - Create HTTP Servers (we’ll discuss this tomorrow)

### fs package

- **The fs (Filesystem) package is used to read, write, update contents on the filesystem.**

```jsx
const fs = require('fs');
const path = require('path');

const filePath = path.join(__dirname, 'a.txt');

fs.readFile(filePath, 'utf8', (err, data) => {
  if (err) {
    console.log(err);
  } else {
    console.log(data);
  }
});
```
# Why use the `path` library?

1. Cross platform joins (Windows has Users\kirat\dir , linux has Users/kirat/dir)
2. Gives you a bunch of helper functions (dirname)
3. Normalises paths (Converts `/Users/kirat/Proejcts/../../Projects` to `/Users/kirat/Projects`
