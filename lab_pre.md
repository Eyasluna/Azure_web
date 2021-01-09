## Unit0 
### Assignment 1

1. identify by reading carefully the errors in this java program
```java
 public class P1 { 
        System.out.println("Hello!");
        public static void main(String[] args) {
            System.out.println("World!");
        }
    }
 ```
 

2. identify by reading carefully the errors in this java program
```java
public class Test {
        public static void main(String[] args) {
            int[] arr = {1, 2, 3};
            for (int i = 0; i <= arr.length; i++) {
                System.out.println(arr[i]);
            }
        }
    }
```


3. The following program returns the biggest intger of given three. 
```
Example 1:
	Input:  num1 = 1, num2 = 9, num3 = 0
	Output: 9
	Explanation: 
	return the Max of them.
Example 2:
	Input:  num1 = 1, num2 = 2, num3 = 3
	Output: 3
	Explanation: 
	return the Max of them.
```
However, the program has synatx and logical errors. Find and fix them
```java
public class Main {
    public int maxOfThreeNumbers(int a, int b, int c) {
        if (a >= b || a >= c) {
            return a;
        } else if (b >= a || b >= c) {
            return b;
        } else 
            return c;
        }
}
```

Correct: 
```java
public class Main {
    public int maxOfThreeNumbers(int a, int b, int c) {
        if (a >= b && a >= c) {
            return a;
        } else if (b >= a && b >= c) {
            return b;
        } else {
            return c;
        }
    }
}
```
