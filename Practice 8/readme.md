
1. Write a function that will check whether the first character in a string is uppercase or not.
Example of work:
upperCase('regexp');
upperCase('RegExp');
String's not starts with uppercase character
String's starts with uppercase character


2. Write a function that accepts string data and checks whether it matches the email. All characters in different positions are considered valid.
Example of work:
checkEmail("Qmail2@gmail.com");
true


3. Write a regular expression that will find a single d followed by one or more b followed by a d in the text. Remember the found b and the next d after them. Consider upper and lower case.
Example of work:
For string "cdbBdbsbz" result ["dbBd", "bB", "d"]


4. Write a regular expression that will swap places in the string text of the 2 substrings.
Example of work:
Input String "Java Script"
Output “Script, Java”

5. Write a function that will validate the bank card number (9999-9999-9999-9999).

6. Write a function that accepts string data and checks whether it matches the email.
Requirements:
• Numbers (0-9).
• Only Latin letters in uppercase (A-Z) and lowercase (a-z) cases.
• Only "_" and "-" symbols are allowed in the email body. But they cannot be the 1st character of an email.
  • The symbol “-” cannot be repeated.

checkEmail('my_mail@gmail.com');
Email is correct!
checkEmail('#my_mail@gmail.com');
Email is not correct!
checkEmail('my_ma--il@gmail.com');
Email is not correct!

7. Write a function that checks the correctness of the login. The correct login is a string of 2 to 10 characters, containing only letters and numbers, the number cannot be the first. The function should take a string and find all the numbers in that string, including floating-point numbers (eg 3.4).
Example of work:
checkLogin('ee1.1ret3');
true
1.1, 3

checkLogin('ee1*1ret3');
false
1, 1, 3