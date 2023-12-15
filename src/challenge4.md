#### Requirements
In a markdown or text file called `challenge4.md` or `challenge4.txt`, write an explanation of
1. **What `First Class` functions are**
  
   A 'First Class' function refers to its ability to be treated as a first-class object (also referred to as first-class citizen) because it supports all of the operations that other objects are allowed.
    
2. **How this concept applies in JS.**

   In JS, a First Class function can be:
  - *Stored in a variable*
    
        function greet(name) { 

        return `Hi, ${name}!` 
        }
    
    const greeting = greet('Elena');
    
  - *Passed as an argument to a function*

        function fullGreeting(greet, name) { 
    
          greet(name) 
        }
    
    fullGreeting(greet, 'Elena')
    
  - *Returned as a value by functions*

        function createGreeting() { 
    
          return function greet(name) { 
    
            return `Hi, ${name}!`
            }
        }
  - *Be stored in a data structure (i.e. an array)*

        function add(number1, number2) {
            return number1 + number2
        }
    
        function multiply(number1, number2) {
            return number1 * number2
        }
    
        const functionsArray = [add, multiply]
  
3. **What the difference is between declaring a function and calling it**
   
   Bonus: give examples for each explanation
