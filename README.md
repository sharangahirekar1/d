### d-zy ###
Shorthand for dom-manipulation 

## Creating elements
let div = d.el.cr8('div');

## Selectors 
# get element by Id
let root = d.el.id('root');
# query selectors
single element with query
let listElement = d.el.q('.unordered-list-item');
multiple elements with query
let listElements = d.el.qA('.unordered-list-item');
# get by className
let elements = d.el.clA('unordered-list-item');
# get by tagName
let elements = d.el.tgA('li');




## For adding Styles
# styling single element
d.el.s(element,{
  cursor:'pointer',
  color:'grey',
  backgroundColor:'white'
})

# for styling multiple elements
let elements = [element1,element2,element3]
let styles = {
  paddingLeft:'10px',
  border:'1px solid grey'
 }
d.el.sM(elements,styles)
 
 
 ## local storage 
 # set item in local storage
 d.l.s('auth','some gibberish text...');
 let obj = {
    name:'Sharang'
    hobby:'reading'
  }
 Stringified set local storage
 d.l.sS('info',obj)
 
 # get from local storage
 let key = d.l.g('auth');
 
 get parsed item from local storage
 let info = d.l.gP('info');   // if not found return empty object
 
