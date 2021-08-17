# HTML & CSS

docsify extends Markdown syntax to make your documents more readable.

## CSS
### Selector

|     Type     |      Example      |        Description        |
|:------------:|:-----------------:|:-------------------------:|
|   Universal  |         *         |        All Element        |
|     Type     |       input       |          input element          |
|     Class    |       .class      |                           |
| ID           | #id               |                           |
| Attr         | input[attr=value] |                           |
| Group        | div,span          | both <div> <span>         |
| Child        | ul>li             | all li which under ul |
| Sibling      | p~span            |                           |
| Adjacent     | h2+p              |                           |
| Pseudo Class | a:visited         | all visited <a>           |
| Pseudo Ele   | p::first-line     | first line of all <p>     |
  
### Conditional Rules
- @supports
- @media
- @document
```css
@supports (display: grid) {
            section h1 {
                background-color: green;
                color: white;
                padding: 15px;
            }
        }
@media screen and (max-width: 700px) {
            section {
                background-color: green;
                color: white;
                padding: 15px;
            }
        }
@-moz-document url("http://localhost/GfG/document-rule.html") {
            section h1 {
                background-color: green;
                color: #fff;
                padding: 15px;
            }
        }
```
### Animation
- keyframe
```css
div
{
width:100px;
height:100px;
background:red;
position:relative;
animation:mymove 5s infinite;
}
@keyframes mymove
{
0%   {top:0px;}
25%  {top:200px;}
50%  {top:100px;}
75%  {top:200px;}
100% {top:0px;}
}
```
## HTML


