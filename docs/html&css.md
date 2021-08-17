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
## HTML


