[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/GDPVb20V)
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

This function returns the largest number in a given array. It first determines if the array size is 1 which will then result in the only number in the array being returned as it is the biggest number. If this is not the case, then it will make a variable called foo that is made up of the fuction mystery with the inital array minus the first element. Then it will check if the variable foo is bigger than the first value in the array, and if so it will return foo resulting in recurrsion. This will continue until foo is not larger than the first element and will result in the function returning the largest value in the array. When the array has elements that aren't numeric characters, the function will return values based on the logic used in comparing those elements to each other that javascript uses.
