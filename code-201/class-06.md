# Domain Problem is the hardest part in programming, 
- its complication lies in when you can’t really see what you are trying to build very clearly.
- understanding the problem is the most critical piece to the equation.
- you can enhance your understanding of problem domain by; Make the problem domain easier, and Get better at understanding the problem domain.

# Objects:
Objects group together a set of variables and functions to create a model of a something you would recognize from the real world.
### in objects :
- variable becomes property
- function becomes method.
- name of variables and functions in an object called key.
- inside object (key-value).
- The value of a property can be a string, number, Boolean, array, or even another object. The va lue of a method is always a function.
### creating an object using literal notation.
```
var object = {
    key : value,
     key : value,
      key : value,
       key(functionName) : value( function(){
           statements;
           return;
       }),
       } ;
``` 
### Accessing an object
> var varName = object.property/method name;

## Document Object Model (DOM):
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window.

As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.

### DOM Tree:

![DOM Tree](./img/DOM_Tree.png)


> Methodes that find that find elements in the DOM Tree called DOM queries.

> for a list of decument objects in HTML : [Document Object](https://www.w3schools.com/jsref/dom_obj_document.asp
)

> more information about OBjects : [Java Script book Chp 5](https://slack-files.com/files-pri-safe/TNGRRLUMA-F01PDPSKG73/javascript_and_jquery_interactive_jon_du.pdf?c=1615069719-e562efb668b64923)