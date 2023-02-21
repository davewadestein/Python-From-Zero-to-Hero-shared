# Chapter 1: Working with Numbers in Python

<details>
  <summary><b>Learning to code?</b> Start here to learn about <i>expressions</i> and <i>variables</i>!</summary>
<br>
  This section discusses how we work with numbers and <i>numeric expressions</i> in Python. If you haven't written code before,
  there are several concepts that you'll need to understand. If, on the other hand, you already know how to code, this section will
  likely be review, and you may safely omit it.
  
  <h2>Simple numeric expressions</h2>
  If you open up the Python REPL (Read-Evaluate-Print-Loop), you will essentially be able to have a "conversation" with Python.
  The REPL provides a prompt that looks like this: <br/><br/>
  >>><br/><br/>
  You can type any Python code into the REPL, and Python will run it for you. Before we look at Python code, it will be helpful to
  start by using Python as a simple calculator:
  <pre>
  >>> 2 + 2
  4
  >>> 5 - 2
  3
  >>> 3 * 7
  21
  >>> 11.7 / 5
  2.34</pre>
  
  Each line we typed above is considered a <i>numeric expression</i>. That is, each line contains some numeric <i>literals</i>
  (i.e., literally numbers) combined with Python arithmetic <i>operators</i> (in this case, + for addition, - for
  subtraction, * for multiplication, and / for division–there are other operators, and we'll introduce those later). You may have
  noticed that the first three lines operated on <i>integers</i> (whole numbers), often called <i>ints</i> for short.
  
  On the other hand, one of the numbers in the final line, as well as the result of the division, are decimal numbers. <i>Decimal
  numbers</i> are numbers which contain a decimal point. In Python (and other programming languages), these numbers are called
  <i>floating point numbers</i>, or <i>floats</i> for short.
  
  <h2>Variables</h2>
  Using Python as a calculator can be useful (e.g., we might prefer to use Python rather than pulling out our phone to do numeric
  caluclations) and perhaps seems interesting, but if we want to write code, then the first concept we need to understand is the
  idea of <i>variables</i>. A <i>variable</i> can be considered a named box into which we put some information. For now, we will
  demonstrate by storing numbers in our variables, but later on we'll see that we can store things other than numbers in our 
  variables.
<p/><p/>
Suppose we want to store the current year in a variable. We do this by writing an <i>assignment statement</i>, which looks like this:
<pre>
year = 2023
</pre>
  In English, that assignment statement means "create a variable named <b>year</b> and store the number 2023 in it." Note that while
  it may <i>look like</i> it says "year is equal to 2023" (much like you might see in a math textbook or similar), it does not, in
  fact, say that. Instead, it's an important action in computer programming which can also be thought of as an imperative–SET or
  MAKE the value of the variable <b>year</b> to 2023. If the variable <b>year</b> had not previously existed, it is created as a
  result of this assignment statement.
  <p/><p/>
  It will helpful at this point to define a <i>comment</i>. A <i>comment</i> in a programming language is a way to write a "note" 
  that Python ignores. (Comments are for humans, not the computer.) Python's comment character is <i>#</i>. If
  we write a <i>#</i>, then it and any text after it on the line are ignored by Python. So from now on, when we write code, we will
  often follow the code with a comment explaining what the code does, like so:
<pre>
year = 2023     # create a variable named year and store the value 2023 in it
</pre>
  As we saw previously, the assignment statement above puts 2023 into the variable <b>year</b>.
  Suppose we now <i>ask</i> Python what is inside the variable <b>year</b>...we can do this by typing the variable's name and
  pressing the RETURN/ENTER key, like so:
<pre>
  >>> year
  2023
</pre> 
  So this variable gives us a way to store a value and retrieve it later. We can, if we wish, store a different value in <b>year</b>:
<pre>
  >>> year = 1999     # overwrite the existing value of year with a new value
  >>> year
  1999
</pre>
  Any time we need to store some number for later retrieval, we can create a new variable. We don't need to tell Python what type of
  number we will put in the variable-we just put the number into the variable, and Python takes care of the rest:
  <pre>
  >>> cost = 14.99     # create a variable named cost and put the floating point value 14.99 into it
  >>> cost
  14.99
  </pre>
  <b>---END OF LEARNING TO CODE SECTION---</b>
</details>

(__NOTE:__ this book contains many sections like the above which are aimed at non-programmers. Programmers who want a quick
  introduction to Python may safely skip these __Learing to code?__ sections.)
  
Like other languages you may be familiar with, Python's basic numeric types are <i>int</i> (integer) and <i>float</i> (floating
point). We can create an int variable <b>quantity</b> and a float variable <b>price</b>, like so:
<pre>
>>> quantity = 5     # quantity will contain 5, an int
>>> price = 19.99    # price will contain 19.99, a float
</pre>
We can then inspect the values of these variables:
<pre>
>>> quantity
5
>>> price
19.99
</pre>
<details>
  <summary><b>Coding Corner</b> Python is dynamically typed!</summary>
  If you're coming from a language like Java, C/C++, or Go, you likely are familiar with <i>static typing</i>. This is the idea
  in those languages (and many others), that one must declare a variable (and its associated type) prior to using the variable.
  <p/><p/>
  In Java we would declare the quantity and price variables like so:
  <pre>
  int quantity = 5;
  float price = 19.99;</pre>
  You no doubt also know that the types of the variables declared (and defined) above are <i>fixed</i>. You cannot put any other type
  of data into them. Python, on the other hand, is dynamically typed, so Python will not stop us from replacing the value of a
  variable with data of a different type:
  <pre>
  >>> cost = 10
  >>> cost = 'one half' # A Python string, which we will introduce in the next chapter...
  >>> cost
  'one half'</pre>
  Even though Python does not prevent us from doing the above, <i>we</i> should stop ourselves from doing it. Variables have a
  purpose, which we communicate to the reader via the name of the variable. A variable we no longer need should not be re-purposed
  and if we follow that rule we're much less likely to overwrite the value of a variable with a different type (leading to confusion
  or an error down the line).
  <br/><br/>
  <b>---END OF CODING CORNER---</b>
</details>
