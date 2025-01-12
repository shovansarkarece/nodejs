# Path Module
- **To import path module we use this code**
`import path from 'path'`
# join two or more file
- **It is useful when we use server side rendering as well template engine**
```
const fullPath = path.join('/path','index.py','file.java')
console.log("files join = ",fullPath)
```
#### Output
```Joined Files Together is \path\index.py\file.java```
# Absolute path
- **Absolute path will return the whole path where our file is located**
```
const absolutePth = path.resolve();
console.log(`We are currently working on ,${absolutePth} directory`)
```
#### Output
```
We are currently working on F:\CODE\JavaScript\nodjs\path_module directory
```
# Extension name 
```
const extname = path.extname('resume.docx')
console.log("extname = ",extname)
/// Output:extname =  .docx
// Check that file is available or not
if(extname == '.docx'){
     console.log(`this is a ${extname} file`)
 }
else
{
    console.log(`this is not a ${extname} file`)
}
/// Output:this is a .docx file
////Another Example
const extName = path.extname('arijit.mp3')
console.log(extName)
/// Output:.mp3
```
# file directory
- **It(`dirname`) will return the immediate file directory**
```
 const directoryName = path.dirname('/path_module/index.js')
 console.log(directoryName)
/// Output:/path_module
 const directoryName1 = path.dirname('/path_module/')
 console.log(directoryName1)
/// Output:/
```
# Base path
- **It(`basename`) will return the immediate file name or immediate file directory name**
```
const basepath = path.basename('/public/java/constructor.java')
console.log(basepath)
///Output:constructor.java
const basepath1 = path.basename('/public/java/JS/')
console.log(basepath1)
///Output:JS
const basepath2 = path.basename('/public/java/')
console.log(basepath2)
///Output:java
```
