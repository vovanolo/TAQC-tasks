
1. Test the addition of the number 0.1 to the number 0.2 with the result 0.3.

2. Perform testing of the given userList array.
1) Test whether there is an “admin” element in the array
2) Test whether the first element in the array is “Nick”
3) Test whether the last element in the array is “new_user_2”
4) Test the statement that the length of the array is 5
5) Test the statement that the 3rd element of the array has type string
6) Prove the statement that the 8th element of the array does not exist.

const userList = ['Nick', 'Kate', 'quest123', 'admin', 'new_user_2'];

3. Create a calcCircle.js file that contains 2 functions for calculating the circle length getCircleLength(radius) and circle area getCircleArea(radius). Export functions.
Create a file calcCircle.test.js in which you need to test the specified functions.
1) Test the function getCircleLength() with argument 22, check the assertion that the length of the circle is 138.2 when calculated with accuracy to 1 decimal place.
2) Test the function getCircleArea() with argument 9, verify the assertion that the approximate area of the circle is 254.47.
3) Test both functions with no arguments passed.

function getCircleLength(radius) {
     return 2 * Math.PI * radius;
}

function getCircleArea(radius) {
     return Math.PI * radius ** 2;
}


4. Create a food.js file that contains the function filterFoodPrice(food, min, max), which filters the array of products by price. Moreover, food is an array of objects with the type and price of the product, min is the set minimum price of the product, max is the set maximum price of the product Execute export function.
function filterFoodPrice(food, min, max) {
     return food.filter(element => element.price >= min && element.price <= max);
}

const food = [
     { kind: 'potato', price: 10 },
     { kind: 'bred', price: 16 },
     { kind: 'pepper', price: 27 },
     { kind: 'banana', price: 32 },
     { kind: 'lemon', price: 50 }
];

Create a file food.test.js in which you need to test the function for the given array food with arguments min = 12, max = 40.
1) Test whether the expected length of the sorted array 3 corresponds to the actual length.
2) Test whether the sorted array contains the object { kind: 'pepper', price: 27 }.
3) Test whether the sorted array contains 2, 3, and 4 elements of the original food array.
4) Test whether the price property of the 1st element of the sorted array is greater than min.
5) Test whether the price property of the 3rd element of the sorted array is smaller than the max value.
6) Test the assertion that the sorted array does not contain the element { kind: 'lemon', price: 50 }.
7) Propose and test at least 2-3 of your statements for the given function and food array.