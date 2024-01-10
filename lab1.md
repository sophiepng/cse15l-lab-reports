# Lab Report 1

## cd Command
**1. No Arguments**
```
[user@sahara ~/lecture1]$ cd
[user@sahara ~]$ 
```
* The working directory was `/home/lecture1`.
* I got this output because .
* This output is/is not an error because

**2. Path to a *directory* as argument**
```
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$ 
```
* The working directory was `/home` which was changed to `/home/lecture1`.
* I got this output because
* This output is/is not an error because

**3. Path to a *file* as argument**
```
[user@sahara ~/lecture1]$ cd Hello.java
bash: cd: Hello.java: Not a directory
```
* The working directory was
* I got this output because
* This output is/is not an error because



## ls Command
**1. No Arguments**
```
[user@sahara ~]$ ls
lecture1
```
* The working directory was
* I got this output because
* This output is/is not an error because

**2. Path to a *directory* as argument**
```
[user@sahara ~]$ ls lecture1
Hello.class  Hello.java  messages  README
```
* The working directory was
* I got this output because
* This output is/is not an error because

**3. Path to a *file* as argument**
```
[user@sahara ~/lecture1]$ ls Hello.java
Hello.java
```
* The working directory was
* I got this output because
* This output is/is not an error because


## cat Command
**1. No Arguments**
```
[user@sahara ~]$ cat

```
* The working directory was
* I got this output because
* This output is/is not an error because

**2. Path to a *directory* as argument**
```
[user@sahara ~]$ cat lecture1
cat: lecture1: Is a directory
```
* The working directory was
* I got this output because
* This output is/is not an error because

**3. Path to a *file* as argument**
```
[user@sahara ~]$ cat lecture1/Hello.java
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
* The working directory was
* I got this output because
* This output is/is not an error because

