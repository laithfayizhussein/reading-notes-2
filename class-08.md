CSS Layout:
- If one block-level element sits inside another block-level element, then the outer block is parent element and the insider one is child elemnet.
- position in css:
    - normal flow: static
    - Relative Positioning: Relative positioning moves an element in relation to where it would have been in normal flow.
    - Absolute positioning: you define the position for it .
    box offset:
        - fixed position
        - floating elements: used to display elements side by side.
- When you move any element from normal flow, boxes can overlap. The z-index property allows you to control which box appears on top.
- When you use the float property, you should also use the width property to indicate how wide the floated element should be.
- clear propertyThe clear property allows you to say that no element (withinthe same containing element) should touch the left or righthand sides of a box.
- your design needs to be able to work on a range of different sized screens.
- Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide.
- Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.
- Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.

- Layout Grids:Grids set consistent proportions and spaces between items which helps to create a professional looking design;eg: 960.GS

- CSS Frameworks"
providing the code for common tasks, such as creating layout grids, styling forms.

| Advantages of framwork|disadvantages of framworks|
|--------|-----------|
|avoid repeatation|They often require that you use class names in your HTML code|
|They will have been tested across different browserversions|they often contain more code than you need|


- if two rules apply to the same element then rules that appear later in a document will take precedence over previous rules.
