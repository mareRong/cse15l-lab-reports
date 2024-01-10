# cd
**With No Arguments**
```
{
  [user@sahara ~]$ cd
  [user@sahara ~]$ 
}
The directory stayed at home and did not change because no arguments (path to directory) are being inputted to change the directory.
```
**With a path to a directory**
```
{
  [user@sahara ~]$ cd lecture1
  [user@sahara ~/lecture1]$ 
}
The directory changed from home to lecture1 because we ran a command to change the directory with a path to lecture1. 
```
**With a path to a file**
```
{
  [user@sahara ~/lecture1]$ cd messages/en-us.txt
  bash: cd: messages/en-us.txt: Not a directory
}
It outputted an error message because the cd command can only be run on a directory, not a specific file. 
```
# ls
**With No Arguments**
```
{
  [user@sahara ~/lecture1]$ ls
  Hello.class  Hello.java  messages  README
}
It listed all files and folders that are within the directory lecture1. Since we did not give it an argument, the ls command listed out the files within the directory we are currently in. 
```
**With a path to a directory**
```
{
  [user@sahara ~/lecture1]$ ls messages
  en-us.txt  es-mx.txt  ja.txt  zh-cn.txt
}
```
**With a path to a file**
```
{
  [user@sahara ~/lecture1/messages]$ ls en-us.txt
  en-us.txt
}
```
# cat
**With No Arguments**
```
{
  [user@sahara ~]$ cat

}
It runs forever!
```
**With a path to a directory**
```
{
  [user@sahara ~/lecture1]$ cat messages
  cat: messages: Is a directory
}
```
**With a path to a file**
```
{
  [user@sahara ~/lecture1]$ cat messages/en-us.txt
  Hello World!
}
```
