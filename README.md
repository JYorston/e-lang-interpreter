James Yorston & Nicolas Dilley 
JWGY4, ND274

Addition of Switch Statements

Changes to the program
--------------------

First step was to modify tokens.ml to which we added the Switch and Case statements and added them to the relevant printing functions.

We then extended the Stmt type in sourceAst to support switch and case. A switch having an expression and stmt list of cases, and a case having expr, expr statement list, one of the expressions being the expression of the switch used to match it. 

We modified the pretty printing functions in sourceAst for the new statements. We also modified the parsing function to support both new statements. 

We modified typCheck.ml to support the new statements and to support general functionality of cases e.g. cases cannot be a different type to that of the expression being evaluated in the switch.

The astInterp.ml was the most heavily modified file with new functions being added to support interpreting the switch and case statments.

