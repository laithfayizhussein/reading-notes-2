# Read 14-b
## How to Build a Perfect Team:
- more than three-quarters of an employee’s day is spent communicating with colleagues.
- tudies show that groups tend to innovate faster, see mistakes more quickly and find better solutions to problems. Studies also show that people working in teams tend to achieve better results and report higher job satisfaction.
- If a company wants to outstrip its competitors, it needs to influence not only how people work but also how they work together.
- ‘Teams are more effective when everyone is friends away from work.
- there was nothing showing that a mix of specific personality types or skills or backgrounds made any difference.
- Project Aristotle researchers concluded that understanding and influencing group norms were the keys to improving Google’s teams.
- In the best teams, members listen to one another and show sensitivity to feelings and needs.

# Read 14-a
## Transforms:
- The transform property comes in two different settings, two-dimensional and three-dimensiona.
- syntax:
``` 
selector {
  -transform: property (value);
}
```
- transform Properties:
    - 3D,2D Rotate.
    - 3D,2D Scale
    - 3D,2D Translate
    - 3D,2D Skew.

## Transition and Animations:
- Transitions provide a change from one state to another.
- animations can set multiple points of transition upon different keyframes.
-  determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes..
- not all properties may be transitioned, only properties that have an identifiable halfway point. Colors, font sizes, and the alike.
- nimations can only apply a transition within a single property, not from one property to another.
- To set multiple points at which an element should undergo a transition, use the @keyframes rule.

- Simple CSS3 Transitions:
     1. Fade in:
    >syntax:
    ```
    .fade{
            opacity:0.5;
    }
    .fade:hover {
            opacity:1;
    }
    ```
     2. Change color:
     > syntax:
     ```
    .color:hover{
            background:#53a7ea;
    }
    ```
    3. Grow & Shrink:
    >syntax:
    ```
    grow:hover{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
    }
    ```
    4. 3D shadow:
    > syntax:
    ```
    .threed:hover {
    box-shadow:
        1px 1px #53a7ea,
        2px 2px #53a7ea,
        3px 3px #53a7ea;
    -webkit-transform: translateX (-3px);
    transform: translateX(-3px);
    }

- Refrences for cool Animations examples:
    - [404 animation](https://codepen.io/kieranfivestars/pen/MYdQxX)
    - [buttons animated](https://codepen.io/retyui/pen/ByoaXV)
    - [ Bounce Animation](https://codepen.io/dp_lewis/pen/gCfBv)





