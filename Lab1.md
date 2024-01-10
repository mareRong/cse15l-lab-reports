# cd
**With No Arguments**
```
{
  [user@sahara ~]$ cd
  [user@sahara ~]$ 
}
```
**With a path to a directory**
```
{
  [user@sahara ~]$ cd lecture1
  [user@sahara ~/lecture1]$ 
}
```
**With a path to a file**
```
{
  [user@sahara ~/lecture1]$ cd messages/en-us.txt
  bash: cd: messages/en-us.txt: Not a directory
}
```
# ls
**With No Arguments**
```
{
  [user@sahara ~/lecture1]$ ls
  Hello.class  Hello.java  messages  README
}
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

  It runs forever
}
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
