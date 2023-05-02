Download Link: https://assignmentchef.com/product/solved-comp-348-principles-of-programming-languages-assignment-3
<br>
<ol>

 <li><strong><u>Object Programming with Ruby</u></strong><strong>  </strong></li>

</ol>

<strong> </strong>Question 1- (10 pts)

<strong> </strong>Write a Ruby method <em>double </em>that given an array of integers <em>int_values</em>, uses the Array.each, Array.sort method and code blocks to print each array value and its corresponding double value, in sorted ascending order. For instance, given the array [125, 200, 25, 150, 50], your code should print out the following:

25   50

50   100

125   250

150   300

200   400




<h1>Question 2 (15 pts)</h1>

<strong> </strong>

<ol>

 <li>Write a Ruby method for extracting the digits from Quebec Heath Insurance Card ID called <em>HID_num </em>that given a string <em>str</em>, uses regular expressions and back references to find the first valid card number in the string. A person valid health care number has 4 uppercase letters, followed by 8 digits number (e.g.: RENL18347692).The method should return the individual number as an integer value, or <em>nil </em>if no individual valid card number is found.</li>

</ol>

Examples:

<em>HID_num </em>(“SALZ18347692 SALZ62487931”) # returns 18347692

<em>HID_num </em>(“HOuN12345678 HOUN24681357”) # returns 24681357 <em>HID_num </em>(“ChAP62148730 CHA62148730”) # returns <em>nil </em>

<ol>

 <li>Write a Ruby program that reads the name of a text file from the command line, opens the file, reads every line of text in the file, that is a string pass it the method <em>HID_num</em> and prints only the lines that return an accepted number. If your text file contains the three lines above it should only give the first two returns</li>

</ol>

<strong> </strong>

<strong> </strong><strong> </strong>

<strong> </strong>

<h1>Question 3 (25 pts)</h1>




Write a Ruby program in inventory.rb that reads an inventory database file where each line contains an item ID, name, category, and expired date. Your program must process this file and display two lists. The first list displays each category (sorted by category name). For each category, display on a separate line the name of the category, the number of items in the category, and each item name in the category (this list is sorted by category name). The second list displays each item (sorted by item name). For each item, display on a separate line the item’s ID, item name, and expiry date (sorted by item name). Your program will be called with the name of the database file as an argument. For example, running your program on a file called data.txt (“ruby inventory.rb data.txt”) could generate:




<table width="639">

 <tbody>

  <tr>

   <td width="319">% data.txt0002: Bread,CERL, 28NOV170004: Milk, DAIR,07DEC180003: CheeseMozar, DAIR, 01SEP180008: PotatoeRed,VEGT,23NOV17 0004: YOGORT, DAR,03JAN180008: PotatoeRed,VEGT,12DEC170002: Bread, REFF, 28JUN190005: Bacon, REFF,10JUL200002: Bread, REFF </td>

   <td width="319">%ruby inventenry.rb data.txt ERROR 0004: YOGORT, DAR,03JAN18ERROR 0002: Bread, REFFCATEGORIESCERL,1, BreadDAIR,2, CheeseMozar,MilkREFF,2, Bacon, BreadVEGT,1 PotatoeRedITEMS0005: Bacon, 10JUL200002: Bread, 28NOV17, 28JUN190003: CheeseMozar, 01SEP180004: Milk, 07DEC180008: PotatoeRed, 23NOV17  </td>

  </tr>

 </tbody>

</table>




Item IDs must be coded on 4 digit starting from 0000 to 9999, and are separated from item names by a colon and a space. Item names must be composed of 1 or more lowercase and uppercase characters. Category names must be exactly four uppercase letters. Expiry date must be composed of two valid digits for the day of the month and three valid upper case letter of the month name and the last two digits of the year. Category names and expiry date are separated by commas. Lines that do not follow this format should produce an error message.




Items may have an arbitrary number of expiry dates. Each item may only be counted once for each category with the closest expiry date, even if they have multiple expiry date within the category (e.g., PotatoeRed only counts as 1 item for VEGT).You may assume each item has a single unique ID.




While reading in the file, for each invalid line found, your program should output ERROR followed by the invalid line. Next, it should output “CATEGORIES”, followed by the information for each category (in sorted order by category name). Finally, it should output “ITEMS”, followed by the information for each item (in sorted order by item name).




<strong><u>Note:</u></strong> You can make use of (a) Code block, (b) pattern matching, and (c) the sort build-in function of Ruby.




<ol>

 <li><strong> <u>Procedural programming with C</u> </strong></li>

</ol>

<strong> </strong>

<h1>Question 4 (10 pts)</h1>




Write a C function <em>twoStrCompr</em> that takes two arguments of type string. The function <em>twoStrgCompr </em>should return “True” if the first string is alphabetically smaller than the second string argument, “False” otherwise. You may assume that the two strings arguments contains only upper case letters, or lower case letter but not both, and  no blanks or other no alphabetical characters is allowed. Test your function with a suitable main program. Once working properly, convert the function <em>twoStrgCompr</em> to pointer arithmetic syntax, and check that it still behaves in the same way.

<strong> </strong>

<strong><u>Question 5</u> </strong>(20 pts)

<strong> </strong>

<ol>

 <li>Write a C program that: creates and prints out a linked list of strings. Similar to java your program should include the node struct. Test your program for different lists of string.</li>

 <li>Add the following functions to the program above:

  <ul>

   <li>void add_after(node_ptr &amp;list, char a_word[], char word_after[])</li>

  </ul></li>

</ol>

which inserts a node containing “word_after” in the linked list “list”, after the first occurrence of a node containing “a_word”. If “list” does not contain such a node, the function leaves it unchanged.

<ul>

 <li>void delete_node(node_ptr &amp;a_list, char a_word[]) which deletes the first node in “a_list” which contains “a_word”.</li>

 <li>void list_selection_sort(node_ptr &amp;a_list)</li>

</ul>

which sorts a list alphabetically (use your answer to Question 4 to help).




sample input/output might be:

Enter first word (or ‘.’ to end list): though

Enter next word (or ‘.’ to end list): actions

Enter next word (or ‘.’ to end list): speak

Enter next word (or ‘.’ to end list): louder

Enter next word (or ‘.’ to end list): than       Enter next word (or ‘.’ to end list): words       Enter next word (or ‘.’ to end list): .




THE LIST IS NOW:

<h2>       though actions speak louder than words</h2>




AFTER WHICH WORD WOULD YOU LIKE TO ADD AN EXTRA WORD? though

WHICH WORD WOULD YOU LIKE TO ADD? many




THE LIST IS NOW:

<h2>       though many actions speak louder than words</h2>




WHICH WORD WOULD YOU LIKE TO DELETE? than




THE LIST IS NOW:

<h2>       though many actions speak louder words</h2>




AFTER SORTING, THE LIST IS:

actions louder many speak though words

<strong> </strong>

<strong><u>Question 6</u> </strong>(20 pts)




<ol>

 <li>a) Similar to assignment 2, but now using C program, compute series for functions ln (1+ <em>x</em>) and <em>e<sup>x</sup></em> depending on a switch variable <em>s</em>. Write a function that takes in three arguments e.g. function <em>compute-trig</em>(<em>x</em>, <em>s</em>, <em>n</em>), where</li>

</ol>




<em>s</em> is the switch variable that decides which function to evaluate, <em>n</em> is the precision variable and <em>x</em> is the parameter variable. Parameters <em>s</em> and <em>x</em> should be defined as keyword parameters and <em>n</em> should be an optional parameter with default value of <em>n</em>=5. You are not allowed to use any inbuilt functions except functions to check value type. Your program should print an apt error for string and decimal values for <em>s</em> and <em>n</em>. Additionally, there is a limit for <em>x</em> with <em>s</em>=2.

<ol>

 <li>b) Compare between Lisp and C paradigms to compute the functions above, which one you will recommend to learn first for a freshman with no computing background? why?</li>

</ol>

<strong> </strong>