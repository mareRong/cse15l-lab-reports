# cd
**With No Arguments**
```
{
  [user@sahara ~]$ cd
  [user@sahara ~]$
  [user@sahara ~/lecture1]$ cd
  [user@sahara ~]$
}
```

The working directory for the first part is /home, and the second part is /home/lecture1. The directory for the first
part stayed at home and did not change, whereas the directory went back to /home after the cd command was inserted.
Since no arguments (directory path) were being input to change the directory, the cd command went to the home
directory as default.

**With a path to a directory**
```
{
  [user@sahara ~]$ cd lecture1
  [user@sahara ~/lecture1]$ 
} 
```

The directory changed from /home to /home/lecture1 because we ran a cd command to change the directory with a path to 
lecture1.

**With a path to a file**
```
{
  [user@sahara ~/lecture1]$ cd messages/en-us.txt
  bash: cd: messages/en-us.txt: Not a directory
} 
```

The working directory is /home/lecture1. The command outputted an error message because the cd command can only be run on
a directory, not a specific file.

# ls
**With No Arguments**
```
{
  [user@sahara ~/lecture1]$ ls
  Hello.class  Hello.java  messages  README
} 
```

It listed all files and folders that are within the directory /home/lecture1. Since we did not give it an argument, the ls
command listed out the files within the working directory we are currently in.

**With a path to a directory**
```
{
  [user@sahara ~/lecture1]$ ls messages
  en-us.txt  es-mx.txt  ja.txt  zh-cn.txt
} 
```

The working directory is /home/lecture1. The command listed out all files that are within the directory messages because
we input a path to a new directory for the command to list files in the asked directory.

**With a path to a file**
```
{
  [user@sahara ~/lecture1/messages]$ ls en-us.txt
  en-us.txt
}

```
The working directory is /home/lecture1/messages. The command returned en-us.txt because we indicated a specific file as
the argument for the ls command to list.

# cat
**With No Arguments**
```
{
  [user@sahara ~]$ cat
  hi
  hi
}
```
The working directory is /home, and running the cat command on its own duplicates whatever we type into the
terminal. The cat command takes an argument and returns the content within the file provided, and since we do
not have an input argument, the cat command waits for the user to input something and prints out the intake
value.

**With a path to a directory**
```
{
  [user@sahara ~/lecture1]$ cat messages
  cat: messages: Is a directory
}
```

The working directory is /home/lecture 1. The command returned an error because the cat command should be run on a
file, not a directory, so that no content can be outputted.

**With a path to a file**
```
{
  [user@sahara ~/lecture1]$ cat messages/en-us.txt
  Hello World!
} 
```

The working directory is /home/lecture1. The command returned the content within en-us.txt file because we inputted
a path to a file as an argument for the command to retrieve content.
