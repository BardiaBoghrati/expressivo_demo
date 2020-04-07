# expressivo_demo
To run this file, navigate to the directory in which it is contained and execute the following command:<br>
java -ea -jar expressivo.jar

For overview of how to use this system consult <a href="https://ocw.mit.edu/ans7870/6/6.005/s16/psets/ps3/#overview">MIT's OCW page</a>

Example session:
<pre>
>x*x                 "entering an expression"
x*x                  "expression becomes <b>current expression</b> and is echoed back"
>!simplify x=2 y=0   "commands begin with !. Note <i>!simplify</i> does not change the current expression"
4.0                  "here all the variables in expression namely x are assigned so <i>!simplify</i> evaluates 
                      the expression to single number"
>!d/dx               "differentiate with respect to x. Differentiation changes the <b>current expression</b>"
x*1 + x*1            "here you should expect any expression equivalent to the one presented"
>!simplify
x + x                "here the echoed expression can be the one shown 'x+x' or any equivalent expression, maybe '2*x'" 
>!simplify x=0.5
1.0
</pre>
