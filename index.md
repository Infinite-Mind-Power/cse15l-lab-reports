# Lab 3

## Part 1 - Bugs

#### A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown):


### Buggy Program Analysis and Fixes

#### Failure-Inducing Input for the Buggy Program


### JUnit Test: Failure-Inducing Input


 ```
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
```

### Non-Failure-Inducing Input for the Buggy Program
An input scenario that does not induce a failure in the reverseInPlace method could involve an array with a single element, where reversing the array should not change the array content.

  ```
    @Test
    void testReverseInPlace_NonFailure() {
    int[] testArray = {1};
    ArrayExamples.reverseInPlace(testArray);
    assertArrayEquals(new int[]{1}, testArray);
  }
  ```


### JUnit Test: Non-Failure-Inducing Input

```
    @Test
    void testReverseInPlace_NonFailure() {
    int[] testArray = {1};
    ArrayExamples.reverseInPlace(testArray);
    assertArrayEquals(new int[]{1}, testArray);
 }
```

### Symptom
When running these tests, the testReverseInPlace_Failure test is expected to fail due to the buggy behavior of the reverseInPlace method. This failure would typically be highlighted by a JUnit assertion error, indicating that the actual array contents do not match the expected reversed array.


### The Bug and Code Changes
#### Bug Description
The reverseInPlace method incorrectly attempts to reverse the array by directly assigning elements from the end to the start, leading to data loss and incorrect reversal, especially noticeable in arrays with an odd number of elements.


#### Before Code Change
```
    static void reverseInPlace(int[] arr) {
     for(int i = 0; i < arr.length; i += 1) {
        arr[i] = arr[arr.length - i - 1];
      }
   }
```

#### After Code Change
The corrected version of the reverseInPlace method uses a temporary variable to swap elements from the start and end of the array, ensuring correct reversal without data loss.

```
    static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length / 2; i += 1) {
        int temp = arr[i];
        arr[i] = arr[arr.length - i - 1];
        arr[arr.length - i - 1] = temp;
    }
  }

```
#### This fix addresses the bug by correctly reversing the array in place, ensuring that the method behaves as expected for arrays of any length.

