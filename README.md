# JavaSE-Static Methods

See the Udemy course: https://www.udemy.com/course/curso-certificacion-profesional-desarrollador-java-se-11

In Java, a static method is a method that belongs to the class rather than an instance of the class. 

This means that you can call a static method on a class itself, without creating an instance of that class.

Here's a simple example to illustrate:

```java
public class MathUtils {
    // A static method to add two numbers
    public static int add(int a, int b) {
        return a + b;
    }

    // Another static method to multiply two numbers
    public static int multiply(int a, int b) {
        return a * b;
    }

    public static void main(String[] args) {
        // You can call static methods without creating an instance
        int sum = MathUtils.add(5, 3);
        System.out.println("Sum: " + sum);

        int product = MathUtils.multiply(4, 6);
        System.out.println("Product: " + product);
    }
}
```

In this example, add and multiply are static methods of the MathUtils class. You can see in the main method that we call these methods directly on the class, without creating an instance of MathUtils.

Static methods are commonly used for utility functions that don't rely on instance-specific data. They are also used in the context of the singleton pattern or in factory methods.

Remember, a static method can't directly access instance variables or non-static methods of a class because it operates at the class level, not the instance level.
