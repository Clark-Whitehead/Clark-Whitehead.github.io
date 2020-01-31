---
layout: essay
type: essay
title: Smart Questions
# All dates must be YYYY-MM-DD format!
date: 2020-01-30
labels:
  - Software Engineering
  - Learning
  - Asking Questions
---

<img class="ui tiny left circular floated image" src="../images/questions.jpg">

## Why Ask Questions in the first place

No matter what your

## How Software engineers ask questions

## What are "Not Smart Questions"? 

Here is an example of a Not Smart Question

https://stackoverflow.com/questions/36890088/sorting-input-radio-boxes-alphabetically/36891877

"I am trying to sort this items alphabetically but it is not sorting all items as it should be. Can you give me some ideas why it is not working ? Here is my fiddle example."

```
handleAlphaOrder = function() {
    var fieldItem = $('.field_item');
    var sorted = $(fieldItem.toArray().sort(function(a, b) {
        return $(a).find('label').text() > $(b).find('label').text()
    }));

    fieldItem.each(function(i) {
        $(this).after(sorted.eq(i));
    });
};
```

## How to ask "Smart Questions"?

Here is an example of a Smart Question

https://stackoverflow.com/questions/11040472/how-to-check-if-object-property-exists-with-a-variable-holding-the-property-name

"I am checking for the existence of an object property with a variable holding the property name in question."

```
var myObj;
myObj.prop = "exists";
var myProp = "p"+"r"+"o"+"p";

if(myObj.myProp){
    alert("yes, i have that property");
};
```
