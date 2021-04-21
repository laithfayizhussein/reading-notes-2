# CSS Grid:
- CSS Grid Layout (aka “Grid”), is a two-dimensional grid-based layout system that aims to do nothing less than completely change the way we design grid-based user interfaces. CSS has always been used to lay out our web pages, but it’s never done a very good job of it.
- lexbox helped out, but it’s intended for simpler one-dimensional layouts, not complex two-dimensional ones.
- The smaller images (in a grid!) are in the perfect layout to get you started with CSS grid. Grid gives us control over how wide or narrow each of the ‘grid cells’ get. This allows us to maintain a sensible aspect ratio to their height. In this example I’ve used:
> grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
- **Grid Container:** he element on which display: grid is applied. It’s the direct parent of all the grid items.
- **Grid Item:** The children (i.e. direct descendants) of the grid container.
- **Grid Line:** he dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”).
- **Grid Cell:** he space between two adjacent row and two adjacent column grid lines.
- **Grid Track:**The space between two adjacent grid lines.
- **Grid Area:**The total space surrounded by four grid lines.
## Grid Properties:
-  for the Grid Container: 
    - display.
    - grid-template-columns.
    - grid-template-rows.
- for the Grid Items:
    - grid-column-start
    - grid-column-end
    - grid-row-start
    - grid-row-end
    - grid-column
    - grid-row
    - grid-area

##  Regex:
- Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern.
- One of the most interesting features is that once you’ve learned the syntax, you can actually use this tool in (almost) all programming languages ​​(JavaScript, Java, VB, C #, C / C++, Python, Perl, Ruby, Delphi, R, Tcl, and many others) with the slightest distinctions about the support of the most advanced features and syntax versions supported by the engines).
- Flags:
    - g (global) does not return after the first match, restarting the subsequent searches from the end of  the previous match
    - m (multi-line) when enabled ^ and $ will match the start and end of a line, instead of the whole string
    - i (insensitive) makes the whole expression case-insensitive (for instance /aBc/i would match AbC)

