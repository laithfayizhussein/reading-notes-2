# Flex Box:
- to set elements as flexible boxes we set  ` {display:flex} ` on the parent element of the elements we want to affect.
- this causes parent to become flex  container and its children to become flex- items .
- parent `{display:flex}` is acting like block level element in term of how it interacts with the rest of the page .
- default ` flex-direction ` raw :means when I ditermine the parent to be display flex the choldern will appear in raw.
- flex -wrap for the parent 
- we can ditermine to flex specific child and give it a portion 
- flex-shrink: when there is an overflow .
- Prefixing Flexbox:
flex-box ex:

```
.parent {
  display: flex;
  height: 300px; 
}

.child {
  width: 100px;  
  height: 100px; 
}
 ```
 # Javascript Templating:
 - is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source.
 
 ## Mustache:
 - is a logic-less template syntax. It can be used for HTML, config files, source code — anything.
 - is a logic-less template syntax. It can be used for HTML, config files, source code — anything.
 > syntax:
 ` Mustache.render(“welcome , {{name}}”, { name: “bayan” })` 
 - Mustache is NOT a templating engine. Mustache is a specification for a templating language. 

