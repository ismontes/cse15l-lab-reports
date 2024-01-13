
1. `cd` without argument
```
[user@sahara ~/lecture1]$ cd
[user@sahara ~]$
```   
* When `cd` is used without a command it changes the directory back to Home if it's in another directory
* Not an error as it just changes back to home

2. `cd` with a path to a *directory* as an argument
  ```
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$   `
``` 
* Using `cd lecture1` we change our directory from home to the folder Lecture1 which is why after the line runs we get `[user@sahara ~/lecture1]`. It's like our new starting point.
* Not as error

3. `cd` with a path to a *file* as an argument
```
[user@sahara ~/lecture1]$ cd messages/es-mx-txt
bash: cd: messages/es-mx.txt: Not a directory 
```
*We got this line because the txt message itself is a file not a directory which `cd` is used for so it couldn't change into it
*I don't think it would be an error since it was able to run and compile and stated that the file is not a directory

4. `ls` without argument
   ```
   [user@sahara ~]$ ls
   lecture1
   ```
   *The command listed the items in Home which happens to be the folder `lecture1`
   *Not an error

5. `ls` with a path to a *directory* as an argument
   ```
   [user@sahara ~]$ ls lecture1
   Hello.class  Hello.java  messages README
   ```
   *The command listed the items in the Lecture1 folder: `Hello.class  Hello.java  messages README`
   *Not an error

6. `ls` with a path to a *file* as an argument
   ```
   [user@sahara ~/lecture1/messages]$ ls es-mx.txt
   es-mx.txt
   ```
   *The command listed the files that was called, that being only one. Didn't read the contents because that's not part of the function
   *Not an error

7. `cat` without argument
   ```
   [user@sahara ~]$ cat

   
   ```
   *The command when entered prints nothing and changes nothing. Unless you CTRL + C the terminal won't start up again and beings a loop of new lines
   *This is an error because you wont be able to do anything without exiting the terminal

8. `cat` with a path to a *directory* as an argument
   ```
   [user@sahara ~lecture1]$ cat messages
   cat: messages: Is a directory
   ```
   *The command doesn't print the Strings of information of the directory because it isn't a txt.file and instead prompts us that `messages` is a directory
   *Not an error, but stating that it's a directory

10. `cat` with a path to a *file* as an argument
   ```
   [user@sahara ~]$ cd lecture1/messages
   [user@sahara ~/lecture1/messages]$ cat en-us.txt
   Hello World!
   [user@sahara ~/lecture1/messages]$ 
   ```
  *When using `cat` on a file, the program runs and prints out the phrase in English successfully in a new line
  *This is not an error
