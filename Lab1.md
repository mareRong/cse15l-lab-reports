# cd
**With No Arguments**
```
{
  [user@sahara ~]$ cd
  [user@sahara ~]$ 
}
The working directory stayed at home and did not change because no arguments (path to directory) are being inputted
to change the directory.
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
The working directory is lecture1. The command outputted an error message because the cd command can only be run on
a directory, not a specific file. 
```
# ls
**With No Arguments**
```
{
  [user@sahara ~/lecture1]$ ls
  Hello.class  Hello.java  messages  README
}
It listed all files and folders that are within the directory lecture1. Since we did not give it an argument, the ls
command listed out the files within the working directory we are currently in. 
```
**With a path to a directory**
```
{
  [user@sahara ~/lecture1]$ ls messages
  en-us.txt  es-mx.txt  ja.txt  zh-cn.txt
}
The working directory is lecture1. The command listed out all files that are within the directory messages because
we inputted a path to a new directory for the command to list files in the asked directory. 
```
**With a path to a file**
```
{
  [user@sahara ~/lecture1/messages]$ ls en-us.txt
  en-us.txt
}
The working directory is messages. The command returned en-us.txt because we indicated a specific file as the
argument for the ls command to list.
```
# cat
**With No Arguments**
```
{
  [user@sahara ~]$ cat
  hi
  hi
}
The working directory is home, and running the cat command on its own has an empty output. However, we could
continue to type into the terminal, where the same value we inputted will be returned to us as an output.
```
**With a path to a directory**
```
{
  [user@sahara ~/lecture1]$ cat messages
  cat: messages: Is a directory
}
The working directory is lecture 1. The command returned an error because the cat command should be run on a
file, not a directory, so that no content can be outputted.
```
**With a path to a file**
```
{
  [user@sahara ~/lecture1]$ cat messages/en-us.txt
  Hello World!
}
The working directory is lecture1. The command returned the content within en-us.txt file because we inputted
a path to a file as an argument for the command to retrieve content. 
```
