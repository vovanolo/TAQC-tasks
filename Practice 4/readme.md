

1. Implement the calcRectangleArea(width, height) function, which takes 2 parameters, the width of the rectangle width and the height of the rectangle height, and calculates its area. Provide termination of program execution and generation of an exception if non-numeric parameters are passed to the function.
Write code that uses this function and handles possible exceptions.


2. Write the checkAge() function, which will prompt the user to enter his age and generate errors in the modal window in the event that:
- the user entered an empty field (for example, "The field is empty! Please enter your age"),
- a non-numeric value
- the user's age is less than 14 years.
Otherwise, the user gets access to watching the movie.
In the catch block, provide for the output of the name and description of the error.


3. Create a MonthException class whose constructor accepts the message parameter and initializes the name field with the value 'MonthException'.
Implement the showMonthName(month) function, where the month parameter is the sequential number of the month of the year. The function returns the name of the month according to the entered month number. In case of incorrect input, an exception is thrown in the form of an object of the MonthException class with the message 'Incorrect month number'.
Write code that uses this function, provide handling of possible exceptions.
An example of the program:
> console.log(showMonthName(5));
May
> console.log(showMonthName(14));
MonthException Incorrect month number

4. Implement the showUser(id) function, which takes the user id as a parameter and returns an object that contains the value of the passed id. The function also throws an error if a negative id is entered.
Implement the showUsers(ids) function, which accepts an array of user IDs as a parameter, checks each element of the ids array for correctness using the showUser() function, and displays an error message in the event of an exceptional situation. The showUsers(ids) function returns an array of objects where the key values are valid ids elements.

An example of the program:
showUsers([7, -12, 44, 22]);
Error: ID must not be negative: -12
[ {id: 7}, {id: 44}, {id: 22} ]