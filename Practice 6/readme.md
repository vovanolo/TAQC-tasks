1. There is a div element on the HTML page:
     <body>
        <div id="test">First</div>
   </body>
You need to change the content of the element from First to Last. Access the div element in at least 2 ways.

2. There is an image element on the page:
      <body>
        <img class="image" src="dog.jpg">
      </body>
You need to change the image dog.jpg to cat.jpg.
Display the contents of the img tag with the new image in the modal window.

3.
        <body>
            <h2>Article header</h2>
                <div id="text">
                    <p>First paragraph</p>
                    <p>Second paragraph</p>
                    <p>Third paragraph</p>
                </div>
            <p>Another text</p>
        </body>
On the specified HTML page, you need to get all the elements inside the div tag by selector (use the document.querySelectorAll method). And output their content with the paragraph number in the following format:
Selector text 0: First paragraph
Selector text 1: Second paragraph
Selector text 2: Third paragraph

4. On the HTML page there is an unnumbered list with id="list", which consists of 5 elements. In the modal window, it is necessary to sequentially display the content:
1) of the first element of the list
2) the last element of the list
3) the second element of the list
4) the fourth element of the list
5) the third element of the list
Do task 2 in different ways.
Example:
• 1
• 2
• 3
• 4
• 5
Output result: 1, 5, 2, 4, 3

5. For the page
<body>
<h1>I'm a big header!!!</h1>
         <div id="myDiv">
             <p>First paragraph</p>
             <p>Second paragraph</p>
             <p>Third paragraph</p>
             <p>Fourth paragraph</p>
         </div>
         <ul id="myList">
             <li>Make</li>
             <li>me</li>
             <li>horizontal!</li>
         </ul>
         <span>Make me invisible, please!</span>
</body>
Write a script that uses DOM tools to stylize the page as shown on the picture task5.png




6. Given an HTML page:
     <body>
        <input type="text" id="input1" value="Text1">
        <input type="text" id="input2" value="Text2">
   </body>
1) The user alternately enters 2 messages (use prompt()). The 1st message is written in the 1st <input>, the 2nd - in the 2nd.
2) Swap the values of the 1st and 2nd inputs.


7. Write a script that, using DOM tools, will create the following structure of tags and their attributes for an empty HTML page.




<body>
    <main class="mainClass check item">
        <div id="myDiv">
            <p>First paragraph</p>
        </div>
    </main>
</body>