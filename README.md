# js30

This is a 30-days javascript grinding  
1.drum-kit: [https://github.com/ningh98/js30]  
2.clock: [https://github.com/ningh98/js30_CSS-JS_Clock]  
3. CSS variable with JS [https://github.com/ningh98/CSS_variable_with_JS]  
4. js array practice [https://github.com/ningh98/js_array]  
5. Flex Panels Image Gallery [https://github.com/ningh98/flex_gallery]  
6. Ajax type ahead [https://github.com/ningh98/ajax_type_ahead]  
7. js array practice 2 [https://github.com/ningh98/js_array2]  
8. html canvas [https://github.com/ningh98/HTML_canvas]  
9. js dev tool tips [https://github.com/ningh98/js_dev_tool_tips]  
10. Hold_Shift_Check_Checkboxes [https://github.com/ningh98/Hold_Shift_Check_Checkboxes]  
11. Custome_video_player [https://github.com/ningh98/custome_video_player]  
12. Key Sequence Detection [https://github.com/ningh98/key_sequence_detection]

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)


## Overview

This project implements an interactive drum kit using HTML, CSS, and JavaScript. The goal is to create a web application where users can play different drum sounds by pressing specific keys on their keyboard.

### Screenshot

![](./screenshot.png)

### Links

- Live Site URL: [https://ningh98.github.io/js30/]

## My process

### Built with

- HTML
- CSS
- Javascript



### What I learned


```html
<div data-key="65" class="key">
      <kbd>A</kbd>
      <span class="sound">clap</span>
</div>
```
kbd represents a span of inline text denoting textual user input from a keyboard, voice input, or any other text entry device.

to use made up html attribute, for example data-key here, you just have to prefix them with data-

```css
.key {
  transition: all .07s ease;
}
```
look it up on mdn

```js
const removeTransition = (e) => {
    if(e.propertyName !== 'transform') return; 
    
    e.target.classList.remove('playing');
}

const keys = document.querySelectorAll('.key')
keys.forEach(key => key.addEventListener('transitionend', removeTransition))
```
transitionend event



### Useful resources

- [keycode.info]    press key to see keycode

