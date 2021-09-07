# FS (File System) in Node.js
### The fs module enables interacting with the file system for read, write, update and delete files and folder. 
For importing fs module we use require keyword like this <br>
```const fs = require('fs');```<br>
### *fs* has few methods to write,update,delete,rename the file, the code could be like below: <br>
+ *mkdirSync* is used for making directory or folder syntax fs.mkdir(filename) if the folder with same name already exist then it will throw error.<br> 
```fs.mkdirSync("day_1");```
![image](https://user-images.githubusercontent.com/34941297/132303024-57a75076-dd30-46f5-90bc-40699e704c82.png)

+ *writefileSync* for writing in file. If file already exists then it overwrites the existing content otherwise it creates a new file and writes data into it. <br>
```fs.writeFileSync("day_1/hello.txt","hello");```
+ *appendFileSync* is used to add or concatinate content in existing file, it will not overwrite rather append. We need to specify the path of file on which we want to append content<br>
```fs.appendFileSync("day_1/hello.txt"," world appended")``` 
+ *readFileSync* is used to read the content of file. It gives the output in buffer format to convet it in string we use "utf-8".<br> ```fs.readFileSync("day_1/hello.txt","utf-8")```

 ![image](https://user-images.githubusercontent.com/34941297/132302417-be0ac55f-d307-4a51-8df8-43f42847aa9a.png)<br>

+ *renameSync* is used to rename or change the file name. firstly we need to specificy existing file name and then the name with which we want rename <br>
```fs.renameSync("day_1/hello.txt", "day_1/hello2.txt")```
+ *unlinkSync* is used to deleting file.<br> ```fs.unlinkSync("day_1/hello2.txt")```
![image](https://user-images.githubusercontent.com/34941297/132303537-03f68836-f5e1-4b02-bf73-c3157de47f43.png)

+ *rmdir* is used for deleting folder only if it is empty.<br> ```fs.rmdirSync("day_1")```







