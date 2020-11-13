# Innes Java PPK package

# Introduction

This Java package allows you to encode PPK image files from images in standard formats (jpeg, png, ...) and to perform the reverse operation.
These operations are performed with the PpkEncDec class via the 2 methods:

+ `PpkEncDec.encode`

+ `PpkEncDec.decode`

It is also possible to create an image by your own in the form of a `BufferedImage` class image and to encode it in PPK via a variant of the `PpkEncDec.encode` method. Conversely, it is possible to retrieve an image of class `BufferedImage` from a PPK file via a variant of the` PpkEncDec.decode` method.

# Distribution

The distribution contains the following:

+ `ppk.jar` : the jar of the Java package,

+ `javadoc` : the directory which contains the JavaDoc documentation of the package,

+ `ppk.html`: the HTML file which allows direct access to the JavaDoc documentation

+ `examples`: the directory which contains examples of use of `Ppp EncDec` (`PpkEncode.java` and `PpkDecode.java`),

+ `README.md`: this file.

# Usage

To use the package, you must import it in your Java program the following packages (see examples `PpkEncode.java` or `PpkDecode.java`:

````Java
import innes.ppk.PpkEncDec;
````

To compile and run your program, you must include the PPK package with the standard option `--classpath` (or `-cp`) of `javac` and `java` command.


````shell
javac -cp <path>/ppk.jar Program.java
java -cp <path>/ppk.jar Program <args>
````

The examples provided in source are also present in the `ppk.jar`. To execute them you must type:

````shell
java -cp <path>/ppk.jar examples.PpkEncode image.jpg
java -cp <path>/ppk.jar examples.PpkDecode image.ppk jpg
````