## Centering Elements on a page using Margins

This is my favourite bit of CSS. It comes from CSS2.1

It is used to center block-level elements on a page.

`style="`  
`margin: 0 auto;`  
`border:1px red solid;`  
`width:80%;`  
`"`

  - Note - the element needs to have a defined width for the margin auto
    (on the left and right) to center the element.

## CSS Shorthand using Margins as example

  - Note - Shorthand format can vary depending on CSS properties (i.e.
    fonts, margin, background etc.)

Shorthand margin values go clockwise, that's how i remember it:

Top Right Bottom Left

so 0 = top/bottom, and auto = right/left

`margin:0 auto;`

is shorthand for

`margin-top:0;`  
`margin-right:auto;`  
`margin-bottom:0;`  
`margin-left:auto;`

  - Note - if some values are the same, you do not have to repeat the
    values.

Eg.

`margin: 10px; = All sides have margin of 10px`  
`margin: 10px 5px; = Top/Bottom have value of 10px, and Left/Right have 5px`  
`margin: 10px 5px 15px; = Top value is 10px, Left/Right have value of 5px, Bottom has value of 15px`  
`margin: 10px 5px 15px 7px; = Top value is 10px, Right has value of 5px, Bottom has value of 15px, Left has a value of 7px`

-----

'''To be added

1.  Box model: Explanation[1](http://css-tricks.com/the-css-box-model/),
    Image[2](http://xhtml.com/C12742E4-3FD2-4084-9E7F-833805A4157C/box-model.gif)
2.  HTML syntax:
    Explanation[3](http://learn.shayhowe.com/html-css/terminology-syntax-intro),
    Image[4](http://urlnextdoor.com/content-include-images/web1/html-syntax.png)
3.  CSS Syntax:
    Image[5](http://createyoursite.org/wp-content/uploads/2013/01/anatomy-of-a-css-rule.gif)
