# [Locale](https://docs.oracle.com/javase/8/docs/api/java/util/Locale.html) Sensitive String Sort

When you sort students enrolled in a course by name using our online services for on-campus students, [anasis](https://anasis.anadolu.edu.tr/), 
you see that names starting with ö, ç, and ş are listed after the letter Z. So apparently there is something wrong here.

Inspired by this, write a Java application called Sort.java that sorts lines in a file. To sort the data in a file named friends.txt, a user would enter:

```
java Sort friends.txt tr-TR
```

When an application is launched, the runtime system passes the command-line arguments to the application's main method via an array of Strings. 
In the example, the command-line arguments passed to the Sort application in an array that contains two Strings: "friends.txt" and "tr-TR."

The first argument is the file, while the second one is the Locale.
In the repository you can find "friends.txt," which contains 111 student names enrolled in the BIM207 Computer Programming III course.
Output of the program will be a file named "sorted.txt."

To compile your source file, please use [javac](http://docs.oracle.com/javase/8/docs/technotes/tools/windows/javac.html).
Make some research on the internet regarding [locale](https://docs.oracle.com/javase/8/docs/api/java/util/Locale.html) sensitive sorting.

After completing this assignment students should be able to:

* Be aware of locale sensitive operations
* Will be able to sort Turkish names correctly
* Work with command-line arguments
* Use the Locale.forLanguageTag(String) factory method, which was introduced in the Java SE 7 release.

## How to test/grade your programming assignment?

* git clone https://github.com/AnadoluUniversityCeng/bim207-pa1-Pinokyo
* cd bim207-pa1-Pinokyo
* javac Sort.java
* java Sort friends.txt tr-TR
* FC sorted.txt expected.txt

