# Lab 3

## Part 1 - Bugs

#### A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown):


### Buggy Program Analysis and Fixes

#### Failure-Inducing Input for the Buggy Program

## Failure-Inducing Input for the Buggy Program

The `reverseInPlace` method in the given `ArrayExamples` class contains a bug that leads to incorrect behavior when attempting to reverse an array in-place. The bug is particularly evident with arrays of odd lengths.

### JUnit Test: Failure-Inducing Input

```java
import org.junit.jupiter.api.Test;
import static org.junit.jupiter.api.Assertions.*;

class ArrayExamplesTest {

    @Test
    void testReverseInPlace_Failure() {
        int[] testArray = {1, 2, 3, 4, 5};
        ArrayExamples.reverseInPlace(testArray);
        assertArrayEquals(new int[]{5, 4, 3, 2, 1}, testArray);
    }

}



