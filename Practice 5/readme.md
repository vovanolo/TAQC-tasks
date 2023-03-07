1. Write a function propsCount(currentObject) that takes an object and determines the number of properties of this object.
For example, for an object
let mentor = {
             course: "JS fundamental",
             duration: 3,
             direction: "web development"
         };
The result should be 3.
propsCount(mentor); // 3


2. Create an arbitrary object that has 5 fields. It is necessary to write the showProps(obj) function, which accepts this object and outputs a list of its properties recorded in an array. Also output an array of object property values.


3. Create the Person class, in which the constructor accepts name and surname parameters, and also contains the showFullName() method, which displays the person's first and last name.
The Student class is derived from the Person class, the constructor of which, in addition to name and surname, accepts the year parameter (the year of admission to the university).
In the Student class, it is necessary to override the showFullName(middleName) method so that not only the first and last names, but also the middle name (middleName) of the student are displayed.
It is also necessary to implement the showCourse() method in the Student class, which will display the student's current course (from 1 to 6). The value of the course will be determined as the difference between the current year (to be determined independently) and the year of admission to the university year.
Example result:
const stud1 = new Student("Petro", "Petrenko", 2015);
console.log(stud1.showFullName("Petrovych")); // Petrenko Petro Petrovych
console.log("Current course: " + stud1.showCourse()); //Current course: 6


4. Create a Worker class that will have a constructor that accepts the following properties: fullName (first and last name), dayRate (rate per day of work), workingDays (number of days worked).
        1) the class must have a showSalary() method that will display the employee's salary. The salary is the product of the dayRate rate by the number of days worked workingDays.
        2) add a private field experience and assign it a value of 1.2 and use it as an additional multiplier when determining the salary - create the showSalaryWithExperience() method. Output the value of the salary with this coefficient.
        3) add getters and setters for the experience field. Set the value experience = 1.5 and display it on the screen.
        4) Output the value of the salary with the new experience.
        5) Create several instances of the class (employees) with different salaries, as shown in the example below. Sort the salary of employees with the most experience in ascending order and output the result in the format: worker_fullName: salary_value
        6) Implement dynamic sorting for any number of worker instances of the Worker class.

Example usage:
let worker1 = new Worker("John Johnson", 20, 23);
console.log(worker1.fullName);
worker1.showSalary();
console.log("New experience: " + worker1.showExp);
worker1.showSalaryWithExperience();
worker1.setExp = 1.5;
console.log("New experience: " + worker1.showExp);
worker1.showSalaryWithExperience();

let worker2 = new Worker("Tom Thomson", 48, 22);
. . . . . .

let worker3 = new Worker("Andy Ander", 29, 23);
. . . . . .

Output example:
John Johnson
John Johnson salary: 460
New experience: 1.2
John Johnson salary: 552
New experience: 1.5
John Johnson salary: 690

Tom Thomson
Tom Thomson salary: 1056
. . . . . .
New experience: 1.5
Tom Thomson salary: 1584

Andy Ander
Andy Ander salary: 667
. . . . . .
New experience: 1.5
Andy Ander salary: 1000.5

Sorted salary:
John Johnson: 690
Andy Ander: 1000.5
Tom Thomson: 1584




5. Create a parent class GeometricFigure that has an empty getArea() method to determine the area and a toString() method to output the class name.
Create 3 descendant classes Triangle, Square, and Circle that inherit from the GeometricFigure class. Each of the child classes has its own implementation of the getArea() method to determine the area of the figure. In the constructors of the child classes, provide the properties necessary to determine the area of the figure, for example, for a circle - the radius r.
Create an external function handleFigures(figures) that will accept an array of objects of child classes figures, check whether the object belongs to the parent class taking into account inheritance, output the name of the created object of the corresponding figure, the calculated area of the figure, and the total area of all figures. You can use the reduce() method to implement the function.

class GeometricFigure {
getArea() {
return 0;
}
toString() {
      return Object.getPrototypeOf(this).constructor.name;
}
      }
Your code. . .

const figures = [new Triangle(4, 5), new Square(7), new Circle(5)];
     console.log(handleFigures(figures));

Example result:
Geometric figure: Triangle - area: 10
Geometric figure: Square - area: 49
Geometric figure: Circle - area: 78.53981633974483
137.53981633974485 // total area