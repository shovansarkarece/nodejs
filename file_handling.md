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
# Append data to file
```
import {readFile,writeFile,appendFile,mkdir,readdir} from 'fs/promises'
const appendtoFile = async (filepath,content) =>{
await appendFile(filepath,content)
console.log("new content added successfully")
}

// await appendtoFile('text.php', ' This is my another brand new content')
```
# Create Directory
```
const createDirectory = async (dirPath) =>{

    await mkdir(dirPath,{recursive:true})
}

// await createDirectory("php/day1/day2");

// python/day1/day2
//Another Example
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
