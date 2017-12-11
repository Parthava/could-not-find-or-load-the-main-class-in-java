# could-not-find-or-load-the-main-class-in-java

### The problem may occur due to the following reasons:

1. You need to install the correct version of the jdk. To know that go to command prompt and type **"java -version"** (without quotes).
2. If your installation is correct then you need to set the environment under: *Advanced system settings --> Environment variables.*
3. Now comes the main part which causes the error. Here I have set the **"class"** & **"classpath"** using a batch file (.bat file). Make sure that your java source file and the batch file are in the same directory. Suppose if your both the files are in E: drive then the code of the batch file looks like this:

```
    @echo off
    E:
    set class="C:\Program Files\Java\jdk1.8.0_121\bin";
    set classpath="C:\Program Files\Java\jdk1.8.0_121\jre\lib\rt.jar";
    color 0a
    pause
```

(Don't copy the **"class"** & **"classpath"** of the batch file from my code. You need to set your own destination from your jdk. As I have described in the video. Save it as "pack.bat").

4. Now open command prompt and go to the location where both the files are present (Suppose E: drive ).
5. Run the batch file. Type: **start " " "pack.bat"** (Exactly same).
6. Now compile and run the java file.

Click [here](https://www.youtube.com/watch?v=6_QNYXDP-1I&feature=youtu.be) to watch the video
