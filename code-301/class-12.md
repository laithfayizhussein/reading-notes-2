# EJSPartials:
- Partials come in handy when you want to reuse the same HTML across multiple views.
- Partials are templates that we can write, that we can include in other templates. For example our html boilerplate, we don’t want to include on every template, that’s not very DRY.
- Partials File Structure Because partials are still templates, we are going to include them in the views folder, in their own sub-directory.
## creating partials :
- inside the “views/partials/ folder
- create a “navbar.ejs”
- only contain the HTML for the nav bar on each page
-  create the same thing for the footer
- now that they are created we can use them in our other .ejs files.
-  Partialscan reuse the same HTML across multiple views. Think of them as functions, make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in. Instead, you define that reusable bundle of code in a file and include it wherever you need it.
-  When making a partial, create a ejs file that will contain only HTML for the partail you are defining, and now you can use the partails in your other ejs templates.
- In EJS, any JavaScript or non-HTML syntax you include in your templates is always surrounded by <% %> delimiters. Use this for a partial in EJS, which is where the partial file is relative to the template you use it in: <%- include( PARTIAL_FILE ) %>
- The <%- %> tags allow us to output the unescaped content onto the page (notice the -). This is important when using the include() statement since you don’t want EJS to escape your HTML characters like ‘<’, ‘>’.
- - Partials are native to EJS.
- Next create the homepage template and include the partial you created in it:

    - Use case for partials would be a nav bar or footer that remains static
    - Go to layout.ejs and within the body tag put another body tag that's for the partial <%- body %>, and underneath it put <%- include('partial/onepartial')%>
    - Then create a new file for the parial/onepartail.ejs. In that new file make a header with a sentence in it and put nodemon in the terminal to see if the partail works. 
    - After you put in nodemon, refresh the web page to see what you wrote in the header

