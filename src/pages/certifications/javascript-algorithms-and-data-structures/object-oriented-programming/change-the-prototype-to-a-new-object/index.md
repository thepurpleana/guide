---
title: Change the Prototype to a New Object
---
## Method 

Instead of adding the properties individually, set the prototype to a new object, like in the example below. 

```javascript
function Cow() { } 

Cow.prototype = {
  numLegs: 4, 
  sound: function() {
    console.log("Moooo!");
  }
};
```



## Solution
```javascript
function Dog(name) {
  this.name = name; 
}

Dog.prototype = {
  // Add your code below this line
  numLegs: 4,
  eat: function() {
    console.log("nom nom nom");
  },
  describe: function() {
    console.log("My name is " + this.name);
  }
};
```
