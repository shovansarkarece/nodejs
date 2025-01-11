# Read File Content
```
import {readFile,writeFile,appendFile,mkdir,readdir} from 'fs/promises'
const readFileContent = async (filepath) =>{
    try {
        const data = await readFile(filepath,'utf-8')
        console.log(data)
    } catch (error) {
        console.error(error)
    }
}
// await readFileContent('Sample.txt')
```
### Another Example of Read Content
```
// Read File Content
// const read_file = async (fileName) => {
//   const data = await readFile(fileName, "utf-8");
//   console.log(data);
// };
// read_file('sample.txt')
```
# Create file
```
import {readFile,writeFile,appendFile,mkdir,readdir} from 'fs/promises'
const createFile = async (filepath,content) =>{
    await writeFile(filepath,content)
    console.log("file created successfully")
}

// await createFile('Inheritance.java','This is inheritance')
// await createFile("superman.js", "This is inheritance");
```
# Another Example of Create file
```
// Create file
// const create_file = async (fileName,content) =>{
//  await writeFile(fileName,content)
//  console.log("File created Successfully..!")
// }
// create_file('ai.py','this is a testing file')
// create_file('App.jsx','this is a React File')
```

# Append data to file
```
import {readFile,writeFile,appendFile,mkdir,readdir} from 'fs/promises'
const appendtoFile = async (filepath,content) =>{
await appendFile(filepath,content)
console.log("new content added successfully")
}
// await appendtoFile('text.php', ' This is my another brand new content')
```
# Another Example of Append data to file
```
// const append_File = async (fileName,content) =>{
//  await appendFile(fileName,content);
//  console.log("extra content added successfully...!")
// }
// append_File('App.jsx',"This is my extra content.")
```
# Create Directory
```
const createDirectory = async (dirPath) =>{
    await mkdir(dirPath,{recursive:true})
}
// await createDirectory("php/day1/day2");
// python/day1/day2
```
# Another Example of Create Directory
```
import {readFile,writeFile,appendFile,mkdir,readdir} from 'fs/promises'
const createDirectory = async (dirPath) =>{
    await mkdir(dirPath,{recursive:true})
}
// await createDirectory("php/day1/day2");
```
# Read Directory Content 
```
const readDir = async (dirPath) =>{
    const files = await readdir(dirPath)
    console.log(files)
}
await readDir('superman')
```
