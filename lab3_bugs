# Debugging
the following code is a method that, in its current state, does not work as intended.:
```
  // Averages the numbers in the array (takes the mean), but leaves out the
  // lowest number when calculating. Returns 0 if there are no elements or just
  // 1 element in the array
  static double averageWithoutLowest(double[] arr) {
    if(arr.length < 2) { return 0.0; }
    double lowest = arr[0];
    for(double num: arr) {
      if(num < lowest) { lowest = num; }
    }
    double sum = 0;
    for(double num: arr) {
      if(num != lowest) { sum += num; }
    }
    return sum / (arr.length - 1);
  }

```
## Diagnosing
**Failure inducing input:** 
```
  @Test
  public void testAverageWithoutLowest() {
    double[] input1 = {3.0, 1.0, 5.0, 6.0};
    assertEquals(14/3, ArrayExamples.averageWithoutLowest(input1), 0);
  }
```
