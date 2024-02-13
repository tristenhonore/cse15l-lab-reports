## Diagnosing
In order to see whether or not the code works as intended we'll run it using different types of inputs that test different possible inputs and confirm it behaves as expected.
**Failure Inducing Input:** 
```
  @Test
  public void testAverageWithoutLowest() {
    double[] input1 = {1.0, 1.0, 5.0, 6.0};
    assertEquals(11.0/2, ArrayExamples.averageWithoutLowest(input1), 0);
  }
```
This test shows the code doesn't work as we intend. The `1.0` appears twice, meaning both should be skipped when averaging the array. The result **should** be 
the sum of `5.0` and `6.0` (11.0) divided by 2. However the program returns the result of 11.0/3.

**Non-failure Inducing Input:**
```
  @Test
  public void testAverageWithoutLowest() {
    double[] input1 = {3.0, 1.0, 3.0, 6.0};
    assertEquals(12/3, ArrayExamples.averageWithoutLowest(input1), 0);
  }
```
This test shows the code working as intended. The code recognizes that `1.0` is the lowest number and only adds `3.0`, `3.0`, and `6.0` then divides by 3.

## [Symptoms]()
As we can see above the program appears to work in some cases but not all, lets look further into the code and see whats wrong.
