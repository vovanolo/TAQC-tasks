
1. Source code:
let arr = ["Tom", "Sam", "Ray", "Bob"];
let [/* Your code */] = arr;
console.log(x); // "Tom"
console.log(y); // "Sam"
console.log(z); // [Bob]
Add the code using destructuring so that lines written in comments appear in the browser console.


2. Source code:
let data = {
    names: ["Sam", "Tom", "Ray", "Bob"],
    ages: [20, 24, 22, 26],
};
let /* Your code */ = data;
console.log(name2); // "Tom"
console.log(age2); // 24
console.log(name4); // "Bob"
console.log(age4); // 26
Add the code using destructuring so that lines written in comments appear in the browser console.


3. Write a function mul() that accepts any number of parameters of different types and returns the product of parameters of type Number.
If there are no parameters of type Number, returns the number 0.
function mul() {
    // Your code
}
console.log(mul(1, "str", 2, 3, true)); // 6
console.log(mul(null, "str", false, true)); // 0
You cannot use the arguments property, but you can add one parameter to the mul() function.

4.
Source code:
let server = {
    data: 0,
    convertToString: function (callback) {
       callback((function () {
          return this.data + "";
       }).bind(this));
    }
};
let client = {
    server: server,
    result: "",
    calc: function (data) {
       this.server.data = data;
       this.server.convertToString(this.notification());
    },
    notification: function () {
       return (function (callback) {
          this.result = callback();
       }).bind(this);
    }
};
client.calc(123);
console.log(client.result); // "123"
console.log(typeof client.result); // "string"
Modify the code using arrow functions so that the code does not use bind() methods.


5. Write the function mapBuilder (keysArray, valuesArrays), which accepts two arrays of the same length. Using these arrays, the function must create a Map object whose keys are values from the first array, and Map values are values from the second array. After that, the function returns this Map object.
Examples of using the function:
let keys = [1, 2, 3, 4];
let values = ["div", "span", "b", "i"];
let map = mapBuilder(keys, values);
console.log(map.size); // 4
console.log(map.get(2)); // "span"