# Lab Report 1

## `cd` Command
**1. No Arguments**
```
[user@sahara ~/lecture1]$ cd
[user@sahara ~]$ 
```
* The working directory was `/home/lecture1`.
* I got this output because the directory changed outside to `/home`. When the `cd` command is used with no arguments it always changes directories to `/home`.
* This output is not an error because the `cd` command correctly changed the home directory if provided no arguments.

**2. Path to a *directory* as argument**
```
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$ 
```
* The working directory was `/home` which was changed to `/home/lecture1`.
* I got this output because the directory was changed to `lecture1` provided as an argument, changing the command line prompt.
* This output is not an error because it was successfully able to change directories into the `lecture1` folder.

**3. Path to a *file* as argument**
```
[user@sahara ~/lecture1]$ cd Hello.java
bash: cd: Hello.java: Not a directory
```
* The working directory was `/home/lecture1`.
* I got this output because `Hello.java` is a file, not a directory, so you cannot change directories into the file.
* This output is an error because the `cd` command could not run, and instead returned an error statement that `Hello.java` is not a directory. The current working directory stays the same.

&nbsp;

## `ls` Command
**1. No Arguments**
```
[user@sahara ~]$ ls
lecture1
```
* The working directory was `/home`.
* I got this output because the `ls` command listed the files and directories within the current working directory if there are no arguments provided.  In the `/home` directory is the `lecture1` folder.
* This output is not an error because it correctly listed the files and directories within the current working directory, if provided no arguments.

**2. Path to a *directory* as argument**
```
[user@sahara ~]$ ls lecture1
Hello.class  Hello.java  messages  README
```
* The working directory was `/home`.
* I got this output because it listed all the files and directories from the argument `lecture1`, which were `Hello.class`, `Hello.java`, `messages`, and `README`.
* This output is not an error because the command correctly ran and produced the list of files and directories from the given directory.

**3. Path to a *file* as argument**
```
[user@sahara ~/lecture1]$ ls Hello.java
Hello.java
```
* The working directory was `/home/lecture1`.
* I got this output because it listed the files in the given argument of `Hello.java`, which was the file itself.
* This output is not an error because the command listed the files from the given argument, which was the `Hello.java` file. 

&nbsp;

## `cat` Command
**1. No Arguments**
```
[user@sahara ~]$ cat

```
* The working directory was `/home`.
* I got this output because there was no argument provided, so the `cat` command returns nothing and copies any other user input until the process is exited.
* This output is an error because it cannot print the contents of a file if there is no file name provided. Thus, it gives empty lines or repeats user input.

**2. Path to a *directory* as argument**
```
[user@sahara ~]$ cat lecture1
cat: lecture1: Is a directory
```
* The working directory was `/home`.
* I got this output because the `lecture1` argument provided is a folder not a file, so the `cat` command could not run and print a file's contents.
* This output is an error because `lecture1` is not a file and cannot be printed by the command, so and error message is returned stating that `lecture1` is a directory.

**3. Path to a *file* as argument**
```
[user@sahara ~/lecture1]$ cat Hello.java
import java.io.IOException;
import java.nio.charset.StandardCharsets;
import java.nio.file.Files;
import java.nio.file.Path;

public class Hello {
  public static void main(String[] args) throws IOException {
    String content = Files.readString(Path.of(args[0]), StandardCharsets.UTF_8);    
    System.out.println(content);
  }
```
* The working directory was `/home/lecture1`.
* I got this output because the `cat` command printed out the contents of the provided `Hello.java` file. 
* This output is not an error because the `cat` command correctly ran and printed out the file that was inputted as an argument.

