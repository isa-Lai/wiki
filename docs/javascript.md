# Java Script

## jQuery
### General

Useful Function
```javascript
//Attribute
$(this).attr('id');//accessor
$(this).attr('id','id_name');//constructor

//css or style
$(this).css("property","value");
```

### Selector
- For selector please check [Selector At CSS & Html](html&css?id=selector)
- Some useful example

```javascript
//position
$('.div:first') //find the first div
$('.div:last')
$('.div:even')
$('.div:odd')

//not
$('input:not(:checked)')

//content
$('.div:contains("content")') //include content
$('.div:has(span)') //include element
```
