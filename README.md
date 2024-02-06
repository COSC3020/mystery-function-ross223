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

This function returns the largest number in a given array. It first determines if the array size is 1 which will then result in the only character in the array being returned as it is the biggest character. Then it will recursively call itself with the array minus the first element until the array foo has 1 element. This element is then compared with all of the other ones to figure out which one is the largest. When an array has elements that aren't numeric characters, the function will return values based on the logic used in comparing those elements to each other that javascript uses.
