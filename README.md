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

This function returns the largest character in a given array. In an array of numbers it will return the largest number. If the array is made out of characters it will convert them to their unicode counterparts allowing for comparisons and will find the furthest letter in the alphabet. In an array of non-numeric strings and numbers, the strings are converted to an always false variable which results in varried outputs based on where the strings are located in the array due to where the comparisons happen during recursion. For instance, an array of [1, 'a', 'b', 1, 2] will return 1 but an array of ['a', 'b', 1, 1, 2] will return b. 
