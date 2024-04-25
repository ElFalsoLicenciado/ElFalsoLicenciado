# Things to keep in mind while coding. _Do's and Dont's_.
1. Use enums instead of integers (might be harder in java to cast to int, but still is a nice convention to have)
2. Avoid nesting more than 3 times by all costs, unless it's a very specifically hard thing to avoid nesting
3. Break your code into functions with descriptive names
4. Write wrapper functions for methods that you're only using 1 parametr for, for showDialogOption for example:
```java
public static int ShowOptionDialog(string name) {
    JOptionPane.showOptionDialog(null, name, "", JOptionPane.DEFAULT_OPTION, JOptionPane.QUESTION_MESSAGE, null, basicData, basicData[0]);
}
```
