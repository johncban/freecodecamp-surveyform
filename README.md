<p align="center">
    <img src="https://image.flaticon.com/icons/png/512/65/65381.png" alt="Logo" width=72 height=72>

  <h3 align="center">FCC: Survey Form</h3>

  <p align="center">
    Pure CSS Survey Form for Perspective Investor.
  </p>
</p>


## Table of contents

- [Preview Demo](#click-preview-for-demo)
- [File Contents](#file-contents)
- [Features](#features)
- [HTML Layout](#html-layout)
- [CSS](#css)
- [Project KB](#project-knowledge-base)
- [Project Sources](#project-sources)


## Click [Preview](https://codepen.io/johncban/full/LYxwQxX) For CodePen
<p align="center">
  <img src="https://raw.githubusercontent.com/johncban/freecodecamp-surveyform/main/assets/readme/survey-form.png" width=900 height=500>
</p>



## File Contents
Simple Assets (with optional image) and Index to show the form.
```
freecodecamp-surveyform$
.
├── assets
│   └── oculus_nyc.png
├── index.html
├── README.md
└── style
    └── form.css
```

## Features

- Animating Background 
- Border Effects
- Radio Control Effects
- Checkbox Control Border Effects

## HTML Layout

The HTML Layout is divided into following:
- Head
  * Body
    * Header
    * Div
      * Form

```
<!DOCTYPE html>
<html>

<head>
  ...
</head>

<body>
    <header class="card-content card">
      ...
    </header>
    <div class="container">
        <form id="survey-form">
          ...
        </form>
    </div>
    <script src="" async defer></script>
    <script src="https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js"><script>
</body>

</html>

```
  




## CSS
The Survey Form's Document Font is Arial for the whole project.
```
:root {
    font-family: Arial, Helvetica, sans-serif;
}
```
The Survey Form's ```body element``` have a unique background that use gradient animation infinite easing.
```
body::before {
    content: '';
    position: fixed;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    z-index: -1;
    background: linear-gradient(
156deg, #f6f6ff70, #797979b4, #626364b6, #ffffff) /*, url(https://raw.githubusercontent.com/johncban/freecodecamp-surveyform/main/assets/oculus_nyc.png)*/;
    background-size: 400% 400%;
    animation: gradient 15s ease infinite;
}
```

## Project Knowledge Base

### [:root](https://developer.mozilla.org/en-US/docs/Web/CSS/:root)
- The HTML's DOM CSS element that have higher specificity or more relevant to the Form's CSS.
### [::before(:before)](https://developer.mozilla.org/en-US/docs/Web/CSS/::before)
- A CSS Pseudo Element that selected first for cosmetic use of the element. In this project, it's use in the ```body element``` for the background.
### [linear-gradient](https://developer.mozilla.org/en-US/docs/Web/CSS/gradient/linear-gradient())
- A CSS function that provide image or color transition between two or more colors. In this project, the ```body element``` use the said function as its ```background``` with [animation](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations/Using_CSS_animations).


## Project Sources

**CSS Input Border Animation**

- <https://codeconvey.com/css-input-border-animation/>

**Inclusively Hiding & Styling Checkboxes and Radio Buttons**
- <https://www.sarasoueidan.com/blog/inclusively-hiding-and-styling-checkboxes-and-radio-buttons/>
