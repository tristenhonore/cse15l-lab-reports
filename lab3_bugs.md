# Debugging
the following code is a method named `averageWithoutLowest`:
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
This code compiles and can be run with an input of an array. At first glance you may or may not see anything wrong with it, but you should always test 
for possible failures within your code. 

---
## [Diagnosing](lab3_bugs_2ndpage.md)
we can see the code and its purpose, now lets attempt to run it with different inputs. 

