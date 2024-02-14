# Lab 3

## Part 1 - Bugs

## A failure-inducing input for the buggy program, as a JUnit test and any associated code:

### JUnit Test: Failure-Inducing Input

```java
import org.junit.Test;
import static org.junit.Assert.assertArrayEquals;

public class ArrayExamplesTest {

    @Test
    public void testReverseInPlace_Failure() {
        int[] testArray = {1, 2, 3, 4, 5};
        ArrayExamples.reverseInPlace(testArray);
        assertArrayEquals(new int[]{5, 4, 3, 2, 1}, testArray);
    }

}
```

## An input that doesn't induce a failure, as a JUnit test and any associated code:

### JUnit Test: Non-Failure-Inducing Input:

```java
@Test
public void testReverseInPlace_NonFailure() {
    int[] testArray = {1};
    ArrayExamples.reverseInPlace(testArray);
    assertArrayEquals(new int[]{1}, testArray);
}
```
