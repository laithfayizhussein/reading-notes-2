# Call Stack
-  A mechanism for a code interpreter (like JavaScript in a web browser) to keep track of its place in a script that calls multiple functions
- Call stack also tracks:
    -  What function is currently running
    -  What functions are called from within that function
- Basic functionality :
    -  When a function is called in a script, the interpreter adds it to the call stack and begins carrying out that   function
    -  Any functions called by that function are adding to the call stack on top of the previous function, and run when the interpreter reaches their calls
    -  When current function finishes, interpreter removes it from the top of the stack, and starts executing from wherever it left off in the previous function.
- if we have an asynchronous method like setTimeout () function will normally be sent to the Call Stack, and the latter will quickly understand that it is an asynchronous function and thus take the return back from it () => console.log (‘’) And assign it to the Web API It counts the time period of 2000ms until it re-transmits, not directly to Call Stack, but to a kind of waiting room known as the Tail or Queue.
- Immediately after assigning setTimeout to the Web API it is passed directly to the next function console.log (‘World’) function on line 3, regardless of what the modes in the asynchronous process in the second line become.
#  avaScript Error Messages

- Reference Errors 
   - Temporal Dead Zone: When trying to use a variable that is not declared
            Fix by declaring the variable before any declaration is made

- Syntax Errors : Fix the error, such as a missing paren

- Range Errors
        - Giving an object an invalid length
            Example - An array cannot have a negative length

- Type Errors - Incompatibility, such as accessing a property in an undefined type of variable
        One of the most common errors

- Debugging Code
    console.log is the easiest and most common
    Add breakpoints to see if code before a certain point is running properly

