
1. There is an <a> link on the HTML page. In the case when the href starts with https://, you need to add the target="_blank" attribute to the link.


2. For a given page, find all <h2> with the head class, make them a green background color, then among the found elements, find the elements with the inner class and set their font size to 35px.
. <h2 class="head">header1</h2>
     <h2 class="head">header2 <span class="inner">inner elem1</span></h2>
     <h2>header3</h2>
     <h2 class="head">header4<span>inner elem2</span></h2>
     <h2>header5</h2>


3. Find the <div> tags immediately after the <h3> and move each <div> element so that it is directly above the <h3>.
    <h3>header1</h3>
    <div>text1</div>
    <h3>header2</h3>
    <div>text2</div>
    

4. There are 6 checkboxes on the HTML page. Write a script that, after the user ticks any 3 checkboxes, makes all checkboxes inactive.