# Solution
here is the original, not working as intended code:
```
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
And here is the code fixed to work as intended:
```
  static double averageWithoutLowest(double[] arr) {
    if(arr.length < 2) { return 0.0; }
    double lowest = arr[0];
    for(double num: arr) {
      if(num < lowest) { lowest = num; }
    }
    double sum = 0;
    int divisor = 0;
    for(double num: arr) {
      if(num != lowest) { sum += num; divisor += 1; }
    }
    return sum / (divisor);
```
the issue with the code was that it was dividing by `arr.length - 1` instead of the number of numbers you are averaging. 
Fixing this requires you create a number, in this case `Divisor` that tracks how many numbers you are actually using for the average.
