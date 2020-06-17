# JavaScript

## Error Handling & Debugging

To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run

### EXECUTION CONTEXT
- GLOBAL CONTEXT : Code that is in the script, but not in a function. There is only one global context in any page.
- FUNCTION CONTEXT : Code that is being run within a function. Each function has its own function context

### VARIABLE SCOPE 

- GLOBAL SCOPE : If a variable is declared outside a function, it can be used anywhere because it has global scope. If you do not use the var keyword when creating a variable, it is placed in global scope

- FUNCTION-LEVEL SCOPE : When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope. 

### ERROR OBJECTS 

When there is an error, you can see all of this information in the JavaScript console I Error console of the browser. 

PROPERTY |DESCRIPTION
------------|----------------------------- 
name        | Type of execution 
message     | Description 
fileNumber  | Name of the JavaScript file 
lineNumber  | Line number of error 

OBJECT | DESCRIPTION 
----------------|---------------------------------------------------------------------------
Error           | Generic error - the other errors are all based upon this erro
Syntax Error    | Syntax has not been followed 
Ref erenceError | Tried to reference a variable that is not declared/within scope 
TypeError       | An unexpected data type that cannot be coerced 
Eval Error      | eva l () function used incorrectly
Range Error     | Numbers not in acceptable range 
URI Error       | encodeURI ().decodeURI(),and similar methods used incorrectly

### HOW TO DEAL WITH ERRORS ?

If you come across an error while writing a script (or when someone reports a bug), you will need to debug the code, track down the source of the error, and fix it. Sometimes, an error may occur in the script for a reason beyond your control. For example, you might request data from a third party, and their server may not respond. In such cases, it is particularly important to write error-handling code

### CONSOLE METHODS 

- conso1e.info() : can be used for general information 
- console.warn() : can be used for warnings
- console.error() : can be used to hold errors 
- console. group () : to write a set of related data to the console
- console.groupEnd () :  indicate the end of the group 
- console. table () :  lets you output showing in a table

 
 