# EJSPartials:
Partials come in handy when you want to reuse the same HTML across multiple views.
Partials are templates that we can write, that we can include in other templates. For example our html boilerplate, we don’t want to include on every template, that’s not very DRY.
Partials File Structure Because partials are still templates, we are going to include them in the views folder, in their own sub-directory.
## creating partials :
    - inside the “views/partials/ folder
    - create a “navbar.ejs”
    - only contain the HTML for the nav bar on each page
    -  create the same thing for the footer
    - now that they are created we can use them in our other .ejs files.


