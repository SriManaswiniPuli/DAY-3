## Scope
- It is the lifetime of a variable
- let and const have block scope
- var has functional or global scope

-  ```js
        {
            var a=10;
            let b=20;
        }
        console.log(a);//10 since global scope
        console.log(b);//not defined since block scope

-   ```js
        function fun(){
            var a=1;
            let b=2;
        }
        console.log(a);//not defined
        console.log(b);//not defined
    

## Difference between undefined and not defined
- Undefined is a value
- Not defined is an error

## Typecasting or Coercion
- Implicit conversion 
  -  Automatically done by javascript
       ```js
        var a=3;
        var b="2"
        console.log(a+b);//32
        console.log(a-b);//-2
- Explicit conversion
  -  which is done by us
        ```js
        var a=3;
        var b="2"
        console.log(a+parseInt(b));//5
        console.log(a-b);//-2

## Tricky
- ```js
        [1,2,3].toString()//'1,2,3'
        [1,2,      3].toString()//'1,2,3'
        [1,2,3]+"abc"//'1,2,3abc'
        NaN*3//Nan
        NaN/3//Nan(Any operation with Nan is Nan)
        typeof(NaN)//'number'
        4*2b//NaN

## == and ===
- == allows typecasting and === does not allow typecasting.So === is faster than ==.
-  ```js
        let a=2;
        let b="3";
        console.log(a==b);//true(as it does typecasting and then compares)
        console.log(a===b);//false(no typecasting it does)
   

# Functions

- ## Normal Function
      
    - ```js
        //function declaration or function definition
       //n is parameter
       //function body{}
      function fun(n){
        return n*2;
      }

      //function call
      //argument -7
      console.log(fun(7));
    </script>

    - If return is not given ,it gives undefined.

- ## Arrow Function 
 

    
        const double=(n)=>{
            return n*3;
        };

    - It returns undefined
    - It can also be written as
        const double=(n)=> return n*3;

    The below is the normal function

     ```js
     function fun(a,b){
            return a+b;
        }
        fun(2+3);
    ```
    The same with arrow function with few lines is as follows-

    ```js 
     const fun=(a,b)=>a+b;
        console.log(fun(2+3));
    ```

    ## DRY RULES
    - Don't 
    - Repeat
    - Yourself

    Code without following DRY Rules-

    ```js
       let a=2;
       let b=3;
       console.log(a+b);
    ```


    Code following Dry Rules which is readable,modular-

    ```js
    const fun=(a,b)=>a+b;
        console.log(fun(2+3));
    ```


## 5 Pillars of Code Quality

- Readability-75%
- Maintainability-Code debt
- Extensibility-it should be able to add new features
- Testability-all the testcases should be able to be tested
- Performance

## Copy by value




--------------------------------------------------





## ES6 features

- let&const
- ``template literal







## Object methods

let salaries{
    John:100;
    Manu:350;
}

Object.keys(salaries)//["John","Manu"]
Object.values(salaries)//[100,350]

-----------------------------

- ctrl+space- shortcut for Autocomplete
- ctrl+shift+p-shortcut to get all other shortcuts(mother of all shortcuts)

## Template literal

- It makes code more readable
- It supports multilines

```.js
  const movieUrl = (domain, genre, year) => {
  return "http://" + domain + "?genere=" + genre + "&year=" + year;
};

console.log(movieUrl("imdb.com", "thriller", 2020));

```
- The below is the code using interpolation and template literal for the above code-
```js
const movieUrl = (domain, genre, year) => {
  return `http://${domain}+?genere=${genre}+year= ${year}`;
};

console.log(movieUrl("imdb.com", "thriller", 2020));
```
### Refactoring

- Quality better but with the same functionality

- The above can be refactored as follows-

```js.
   const movieUrl = (domain, genre, year)
      `http://${domain}+?genere=${genre}+year= ${year}`;
```

## Array destructing

const [t1,t2,t3=80]=[100,200,500];
console.log(t1,t2,t3);//[100,200,800]

- Default value will only be taken if t3 is undefined.
- If not takes t3 value

## Object destructing 
 
- It matches with the key,rather than indexes

- const cart = [
  { name: "apple", price: 0.5, quantity: 4 },
  { name: "banana", price: 0.25, quantity: 6 },
];
 
const newItems = [
  { name: "Cherry", price: 0.75, quantity: 5 },
  { name: "Date", price: 1, quantity: 3 },
];
 
//   Ex 1.1: Combine cart + newItems
const comb = [...cart, ...newItems];
var result = 0;
for (let item of comb) {
  result =result+ item.price * item.quantity;
}
 
console.log("The Total Price of all fruits : " + result);


 
--------------------------------------------------
## SOFTWARE DEVELOPMENT LIFE CYCLE
- 1.Planning -Planned by CEO
- 2.Analysis -2types-Business,Technical
- 3.Design -Designers use Figma Vscode,Adobe Xd,Sketch
- 4.Implementation
- 5.Testing and Integration
- 6.Maintenance















































