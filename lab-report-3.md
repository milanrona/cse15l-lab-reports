## Lab Report 3

---

# Part 1

- I am going to choose avaragewithout lowest methods bug. This method takes a list of integers and returns the mean without the lowest number.

- This test induces a failer

`@Test
  public void testAvarageWithoutLowest() {
    double[] input1 = {4, 4, 6};
    assertEquals(5, ArrayExamples.averageWithoutLowest(input1), 0.1);
  }`


- This input doesn't induce a failer
`@Test
  public void testAvarageWithoutLowest2() {
    double[] input1 = {1, 2, 4, 6, 8};
    assertEquals(5, ArrayExamples.averageWithoutLowest(input1), 0.1);
  }`

- Screenshot of running the junit test
![image_junit](screen_of_junit.png)
(The one failure is from the test i wrote, without the lowest score it should have been 5.0 but since the code was wrong it produced 3.0)

-Fixing the code 

Before: 
` static double averageWithoutLowest(double[] arr) {
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
  }`

After: 
`static double averageWithoutLowest(double[] arr) {
    if(arr.length < 2) { return 0.0; }
    double lowest = arr[0];
    for(double num: arr) {
      if(num < lowest) { lowest = num; }
    }
    double sum = 0;
    for(double num: arr) {
      sum += num;
    }
    return (sum - lowest) / (arr.length - 1);
  }`

  - This fixes the problem since now the method doesn't just loop through the list and take out all the numbers that are equal to the lowest, but rather it subtractes the lowest number from the sum. This works for if the lowest number is negative. This way the lowest only gets taken out once.






---

# Part 2

- I will be choosing grep. 
