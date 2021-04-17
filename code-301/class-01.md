# Responsive Web Design (RWD):
- to build websites suitable for all internt users with different devices and different screen sizes.
 - RWD largely developed by Ethan Marcotte.
 - Responsive and adaptive web design are closely related, responsivs is to to react quickly and positively to any change while adaptive is to be easily modified for a new purpose or situation. using both provids the perfect formula for functional websites.
 - main components of Responsive Design:
    - flexible layouts: building the layout of a website capable of dynamically resizing to any width.
     > formela for determining the flixible layout : target ÷ context = result
     - flexible media: make media scalable, the most use property is e max-width property.
    - media queries: 
        - provide the ability to specify different styles for individual browser and device circumstances.
        - Logical Operators used in Media Queries:and, only and not.
        - Media Features in Media Queries:Height & Width Media Features, Orientation Media Feature, Aspect Ratio Media Features, Resolution Media Feature, color, color-index feature.
        - media query syntax :
![media query syntax](./img/READ1.png)
   

# CSS Floats:
- CSS positioning property, allow the floated elements to remain a part of the flow of the web page.
- float values: 
    - left
    - right
    - none
    - inherent
- floats aer used to create an entire web layout.
- clear property related to float;element that has the clear property set on it will not move up adjacent to the float. 
    - also clear has values: both, left, right, none.
- floating of childs elements affect the parent element by height collapse: if this parent element contained nothing but floated elements, the height of it would literally collapse to nothing.
-  fix the collapse proplem  by clearing the float after the floated elements:
    - The Empty Div Method.
    - The Overflow Method
    - The Easy Clearing Metho
- Problems with Floats:
    - Pushdown
    - Double Margin Bug
    - Bottom Margin Bug 


