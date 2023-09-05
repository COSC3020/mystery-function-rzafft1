[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11736290&assignment_repo_type=AssignmentRepo)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```

##
This function finds the maximum value in an array.
First, it checks to see if the array size is one, and then if true, it returns the single element
Then we create a new array by making a recursive call on our original array and returning all elements in the original array except for the first value. Now we check to see if the value that was sliced from the array is greater than the first element of the original array.
we return whichever value is greater and repeat this process until the array length is 1.
