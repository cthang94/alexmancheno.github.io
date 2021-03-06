# Lab 07

> Aim: Two-dimensional arrays and input files

1. Open up PowerShell and `cd` into your `H:\` drive.

2. Create the following folder structure:
```
lab07
└── src
    ├── Main07.java
    ├── TextFileInput.java
└── bin
├── lab07input.txt
```
You can do so by typing in the following into the PowerShell while in the root of your `H:\` drive:
```
mkdir lab07; mkdir lab07/src; mkdir lab07/bin; New-Item -Name "lab07/src/Main07.java" -ItemType "file"; New-Item -Name "lab07/src/TextFileInput.java" -ItemType "file"; New-Item -Name "lab07/lab07input.txt"
```
 
3. `cd` into your new project, `lab07`.

4. Open up `lab07` with Notepad++.

5. Copy and paste the code from <a href="/Misc/TODO/Main07.java" target="_blank">here</a> into `Main07.java`.

6. Copy and paste the code from <a href="/Misc/Solutions/TextFileInput.java" target="_blank">here</a> into `TextFileInput.java`.

7. Copy and paste the input numbers from <a href="/Misc/Input/lab07input.txt" target="_blank">here</a> into `lab07input.txt`.

8. Fill in the `fillArray()` method. The method should return an m x n matrix containing every number after the **second** number of the input file. The first number of the input file is the number of **rows** while the second number of the input file is the number of **columns**.

9. Wrap the line of code where you use `Integer.parseInt()` with a `try-catch` block inside the `fillArray()` method. Without this `try-catch` block, the program will *halt* if an error is thrown by the `Integer.parseInt()` method call (for example, passing a string that contains at least one non-integer character). 

10. Fill in the `printArrayEven()` method. The method should print only the even numbers of the array. For example, an array like:
```
    1 2 3
    4 5 6
    7 8 9
```
Should print as:
```
    * 2 *
    4 * 6
    * 8 * 
```
11. Compile your program:
```
> javac src/*.java -d bin
```

12. Run your program:
```
> java -cp bin Main07 lab07input.txt
```

13. **Bonus**: create another method called `fillArrayAlternate()` that does the exact same thing as `fillArray()`, but using the `Scanner` and `FileReader` class. 

## Solution
The completed code for this lab can be found <a href="/Misc/Solutions/Main07.java" target="_blank">here</a>.