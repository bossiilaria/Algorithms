
function smallestCommons(arr) {
  /*
 One way to solve this problem is by using the Euclid algorithm: LCM = n1 * n2 / GCD
 Find the GCD first.
  */
  //Sort the array in ascending order
  arr.sort(function(a, b)
  {
    return a -b;
  });
  //  Make a function to build an array where to store all the sequential numbers
  function printAllSequentialNum(min, max)
  {

  var allSequentialNum = [];
  
  for(var i = min; i <=max; i++)
  {
    allSequentialNum.push(i);
  }
  return allSequentialNum;
}
  
  
/*Find the LCM of two numbers num1 * num2 / GCD*/
  function lcm(num1, num2)
  {
      for(var GCD = num1; GCD>0; GCD--)
  
      if(num2 % GCD === 0 && num1 % GCD === 0)
    
      return (num1 * num2) / GCD;//This is the LCM of 2 numbers
  }
  //map the whole array to find the lcm not just between 2 numbers but among all of them
var multiple = arr[0];
    printAllSequentialNum(arr[0], arr[1]).map((num, i) => 
    {
        multiple = lcm(multiple, num);
        console.log(multiple);
    });
    return multiple;


 
  /*
   Alex's solution'
  if (arr[0] > arr[1]) {
    var bigger = arr[0];
    var smaller = arr[1];
  } else {
    var bigger = arr[1];
    var smaller = arr[0];
  }

  function allRangeNumbers(num) {
    for (var i = smaller; i <= bigger; i++) {
      if (num % i !== 0) {
        return false;
      }
    }
    return true;
  }

  var multiple = 0;
  var found = false;
  
  while (!found) {
    multiple += bigger;
    found = allRangeNumbers(multiple);
  }
  
  return multiple;
  */
}


smallestCommons([1,5]);
