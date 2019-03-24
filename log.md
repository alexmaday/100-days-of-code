# 100 Days Of Code - Log

### Day 1: March 20, 2019

**Today's Progress**: Worked on CSS box-shadow generator. Adjusting CSS, hooking up events to range sliders and general cleaning/re-factoring of code.

**Thoughts:** I feel like I'm understanding CSS properties much better, but realize how complex it can really get. I mean look at bootstrap and all that fricking code, but in the end it looks pretty good. I'm making adjustments, but my design eye needs improvement. Layout is dull, but that's what practice is for.

**Link to work:** [CSS box-shadow-toy repo](https://github.com/alexmaday/box-shadow-toy) and [codepen](https://codepen.io/alexmaday/pen/qvpgQz)

### Day 2: March 21, 2019

**Today's Progress**:
* [modify html label markup for styling](https://github.com/alexmaday/box-shadow-toy/commit/d688af3d65650f5bc74a3b0128e7e36967a8d5fd) - modified the labels to separate the attribute's description from its value using span tags.
* [style label description and range value](https://github.com/alexmaday/box-shadow-toy/commit/d688af3d65650f5bc74a3b0128e7e36967a8d5fd) - used floats.
* and [updated the range labels programatically](https://github.com/alexmaday/box-shadow-toy/commit/d9868463564c5c0a1fd5dc4362ddc7cced6fcf08)

**Thoughts**: I feel like I'm solving things, but not in the most elegant way. I know that there's smarter more clever ways to structure code, but I don't know how. But that's what practice is for.

**Link(s) to work**: [CSS box-shadow-toy repo](https://github.com/alexmaday/box-shadow-toy) and [codepen](https://codepen.io/alexmaday/pen/qvpgQz)

### Day 3: March 22, 2019

**Today's Progress**:
My box-shadow generator Works! Yay!

I forgot to [add lengths to shadow's attributes](https://github.com/alexmaday/box-shadow-toy/commit/46edbc3f36c76e0081a0fbd11429dccbe609a128) - one of those careless moments.

**Thoughts**: Still *know* I can do much better. My code is so-called correct, because it works, but it's not good. Tomorrow, I'd like to get back to some freeCodeCamping.

**Link(s) to work**: [CSS box-shadow-toy repo](https://github.com/alexmaday/box-shadow-toy) and [codepen](https://codepen.io/alexmaday/pen/qvpgQz)

### Day 4: March 23, 2019

**Today's Progress**:
I refactored my individual event listeners into one (from each range control to the form). It really didn't matter which range control value got changed, I had visit each one anyway to gather the values. Obvious once I thought about it, guess I've been mostly concerned with making it work. So that got more efficient. 

Also started a bit of work on a reset button. The button does what it means to, moves all range sliders to their default value of 0, but none of the logic for the input event get run of course because a reset event != input event. So I refactored my anonymous function out of my input event handler into a new function called `update` and tried to call that code in my reset event handler. It doesn't work. I need the reset buttons to reset to 0 and *then* have the call to update - but it's working in reverse; update then zero. I also tried `dispatchEvent()` but it didn't work (probably because I don't really understand how to use it.)

**Thoughts**: I think it's quite useful to spend some time actually thinking about your code without your computer in front of you. Today, I was just lying down relaxing trying to describe how events work and what bubbling is. From there, I began to question my approach and that's what got me through today's refactoring.

**Link(s) to work**: 
[use form container to capture events](https://github.com/alexmaday/box-shadow-toy/commit/f25ce7668438a5e260e492abb6ca47baee5e1245) and [codepen](https://codepen.io/alexmaday/pen/qvpgQz)
