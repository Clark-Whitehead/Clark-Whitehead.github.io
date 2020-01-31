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

It's very easy to answer your own questions just by searching google, but only if you can type the correct question.

## Why Ask Questions in the first place

When it comes to tasks such as computer programming, working on a car engine, building a house, curing a patient, or even how to draw a straight line, we should be asking questions to learn.  Each time you asks a question, it should be such a simple question that you can remember it and how to come up with the answer next time.  It's similar to remember someones name.  A name is very simple, it's one word, and you say it over and over again, but the main key here is that you are laser focused on one very simple thing, a name.  Questions need to be like that, or you are missing the entire point of asking a question.  Imagine someone answers you and tells you their name and you just say "ok", and don't process it. You will have to ask again everytime.

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

The above question is too vague.  If they don't have a direction for the problem, then I assume they haven't put much effort into solving it, especially now days, with all the text editors which pretty much debug your code as you type it.  This person was incorrectly appending field-Item S back to his DOM.  At a minimum he should have said, "My sort is working, but I'm not seeing the results."  At least this shows he understands a direction where the problem is coming from.  Finding the right question is like solving a maze. In a maze you try a turn, if it works you keep going, then you try another turn, if it fails, you back up, find another turn and keep going.  In this sense, when you finally can't go any further, at least you should have a map of where you are, so the person helping you knows equatly where you have gotten stuck.

If you don't ask the right question the longterm outcome will be damaging.  It is not enough to simply ask the most vague question, you must be very specific.  There are many reasons for this but two are most important. 

One: If you're not asking a precise question, it means you don't understand the problem, and if you don't understand the problem, then even if someone fixes it for you, you will not learn anything and you will need to ask for help again.

Two: If a programming question is too vague, people will have to read all of your code and process it in order to understand what the problem is.  Personally if someone asks why their code isn't running on more than 150 lines of code, unless they are very good friends of mine, I really don't want to help them, because I know they are being lazy and don't even understand the problem and won't understand my answer.  So if you post a question on a forum and it's vague and the code is long, you won't get many answers.

## How to ask "Smart Questions"?

Here is an example of a Smart Question

https://stackoverflow.com/questions/11040472/how-to-check-if-object-property-exists-with-a-variable-holding-the-property-name

"I am checking for the existence of an object property with a variable holding the property name in question."
"This is undefined because it's looking for myObj.myProp but I want it to check for myObj.prop"

```
var myObj;
myObj.prop = "exists";
var myProp = "p"+"r"+"o"+"p";

if(myObj.myProp){
    alert("yes, i have that property");
};
```

First of all this person has only posted a very small amount of code.  This is perfect.  It shows he knows where the issue was coming from out of his entire program.  He states exactly what he wants to happen from this little bit of code, "checking existence of an object property", and what the error is, "undefined".  The issue here was he wasn't completely familiar with the most up to date libraries of the language he was using, such as "hasOwnProperty()".  But the question was so good that it only takes a person who knows the language fluently seconds to look at the question and code and provide a very simple answer.  This is very similar to the name analogy I mentioned above.  He will not forget the answer to this because his mind is focused one thing only, one small function name.  Imagine if he posted a huge mess of code and has 10 bugs and someone is able to give him answers for all 10 bugs, he will not be able to remember all 10 of those fixes because it is too much information at once.

Ask focused questions

This essay actually teaches you more about how to program than how to ask questions properly.  Here's the key, constantly test your code as you type it, so if you do get stuck, your question will be very specific and precise.
