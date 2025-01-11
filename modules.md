# 1. Core Modules
- **Core modules are built into Node.js and can be used without installing additional packages.**
- **They provide functionalities for common tasks, such as handling files, creating servers, and working with streams.**

### Examples:
- **`fs`: File System module (e.g., reading/writing files)**
- **`http`: For creating HTTP servers.**
- **`path`: For working with file and directory paths.**
- **`os`: Provides operating system-related utilities.**
- **`events`: Implements the EventEmitter class.**
- **`stream`: For working with streams.**
- **`util`: Contains utility functions.**
### Usage:
```
const fs = require('fs');
fs.readFile('example.txt', 'utf8', (err, data) => {
  if (err) throw err;
  console.log(data);
});
```
