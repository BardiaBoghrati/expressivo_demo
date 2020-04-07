# expressivo_demo
To run this file, navigate to the directory in which it is contained and execute the following command:<br>
java -ea -jar expressivo.jar

For overview of how to use this system consult <a href="https://ocw.mit.edu/ans7870/6/6.005/s16/psets/ps3/#overview">MIT's OCW page</a>

Note that this is a system of floating-point expressions and numbers are represented by their closest floating-point value.

Example session:
<pre>
>x*x                                  "Entering an expression"
x*x                                   "Expression becomes <b>current expression</b> and is echoed back"
>3xy                                  "Entering Invalid expression"
ParseError: unknown expression        "System should respond by printing an error message of some sort. Note that
                                       <b>current expression</b> is not updated."
>(x                                   "Unmatched paranthesis"
ParseError: unknown expression
>(x*(x + y))                          "Change <b>current expression</b>"
x*(x + y)                             "The echoed expression is any equivalent form of entered expression" 
>(x*x) + y                            "Change <b>current expression</b> again"
x*x + y
>!simplify x=2 y=0                    "Commands begin with !. Note <i>!simplify</i> does not change the current expression"
4.0                                   "Here all the variables in expression namely x & y are assigned so <i>!simplify</i> evaluates 
                                       the expression to a single number"
>!d/dx                                "Differentiate with respect to x. Differentiation changes the <b>current expression</b>"
x*1 + x*1 + 0                         "Here you should expect any expression equivalent to the one presented"
>!simplify
x + x                                 "Here the echoed expression can be the one shown 'x+x' or any equivalent expression, maybe '2*x'" 
>!simplify x=0.5
1.0
</pre>
