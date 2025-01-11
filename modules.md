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
# 2. Local Modules
- **Local modules are user-defined modules created for specific applications.**
- **These can contain functions, classes, or objects to be reused across the application.**

## Creating and Using a Local Module:
- **Create a file, e.g., math.js:**
```
module.exports.add = (a, b) => a + b;
module.exports.subtract = (a, b) => a - b;
```
## Import and use it:
```
const math = require('./math');
console.log(math.add(5, 3)); // Output: 8
```
# Another example
![image](https://github.com/user-attachments/assets/a9a802eb-bc6c-46bf-8fe1-864694460c1c)

# 3. Third-Party Modules
- **Third-party modules are packages installed via npm (Node Package Manager).These are typically downloaded from the npm registry.**
### Popular Third-Party Modules:
- **express:** A web framework.
- **mongoose:** MongoDB object modeling.
- **lodash:** Utility library for JavaScript.
- **axios:** HTTP client for making API requests.
- **chalk:** For styling terminal text.
### Installing and Using Third-Party Modules:
- **Install the package:**
```
npm install chalk
const chalk = require('chalk');
console.log(chalk.green('Hello, World!'));
```
# Recommended
## 4. ES Modules (ECMAScript Modules)
- **Starting with Node.js 12, Node.js supports ES modules using the .mjs extension or by setting "type": "module" in package.json.**
- **Example:**
- **Create a file, e.g., math.mjs:**
```
export const add = (a, b) => a + b;
export const subtract = (a, b) => a - b;
```
- **Import and use it:**
```
import { add, subtract } from './math.mjs';
console.log(add(5, 3)); // Output: 8
```
