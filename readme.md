<h1 style="text-align: center;">Design Improvement 💻🖥️</h1>

# Introduction

<p> Hello students 👋 In this repository we will check if your assignment passed the requirement. </p>

## Requirements:

1. The final output should similar to this:

![BaseOnThis](https://i.imgur.com/YPKcP0M.png)

2. Add a component similar to this:

![ComponentToAdd](https://i.imgur.com/D2NMWjo.png)

3. We have no access of the assets, feel free to download similar images to google.

---

## Steps:

### 1. First we need to take the pictures from the initial task and put it on a separate folder.

### 2. We will create an HTML file named "index" and write the basic starting HTML tags.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body></body>
</html>
```

### 3. Create a CSS file named "style" and inside the file we will add all the styling of our page.

### 4. Link the CSS to the HTML.

```html
<head>
  ...
  <link rel="stylesheet" href="style.css" />
  ...
</head>
```

### 5. After setting up everything, let's add the first image which will be a figure and we will call it "hero".

```html
...
<body>
  <section class="hero">
    <figure>
      <img src="./assets/hero.jpg" alt="Hero Image" />
    </figure>
  </section>
</body>
...
```

### 6. To make it closely the same with the expected output, we will import the font "Roboto" from google fonts on our CSS file and make some adjustments like padding, margins and background color.

```css
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@100;400;700&display=swap");

* {
  margin: 0px;
  padding: 0px;
}

body {
  background-color: #4ef6ae;
  font-family: "Roboto", sans-serif;
}
```

### 7. Then we will create the next section which we will call "banner-container" and add style and div to make it look like the expected output.

<i>HTML</i>

```html
...
<section class="banner-container">
  <div class="banner">
    <div class="banner-text">
      <h2>COMPLETE EDUCATION SOLUTION</h2>
      <h2>BLENDED & TRADITIONAL LEARNING</h2>
      <p>IN AN INNOVATIVE E-LEARNING ENVIRONMENT</p>
    </div>
    <div class="cta-container">
      <div class="buttons enroll">
        <h2>ENROLL NOW</h2>
      </div>
      <div class="buttons login">
        <h2>LOGIN</h2>
      </div>
    </div>
  </div>
</section>
...
```

<i>CSS</i>

```css
...
.banner-container{
    display: flex;
    justify-content: center;
    position: relative;
    bottom: 110px;
}

.banner{
    background-color: #fff;
    border: 5px solid #000;
    border-radius: 20px;
    height: 180px;
    width: 70%;
    padding: 30px 50px;
    display: grid;
    grid-template-columns: 50% 50%;
    grid-template-rows: 1fr 1fr;
}

.banner-text{
    border-left: 6px solid #525453;
    padding: 9px 0px 9px 12px;
    grid-column: 1/3;
    grid-row: 1/2;
}

.buttons{
    width: 200px;
    background-color: #4EF6AE;
    border-radius: 100px 100px;
    text-align: center;
    padding: 10px 0px 10px 0px;
    font-weight: 700;
    display: flex;
    justify-content: center;
    align-items: center;
}

.login{
    background-color: #E64143;
    color: white;
    margin-left: 30px;
}

.buttons-container{
    display: flex;
    justify-content: center;
    grid-column: 1/3;
    grid-row: 3/4;
}
...
```

### 8. Lastly we will add the component with schools and add styles to make it similar to our expected output.

<i>HTML</i>

```html
...
<section class="schools">
  <div class="component_container">
    <div class="component">
      <div class="component_up">
        <img src="./assets/up-logo.png" alt="UP Seal" />
      </div>
      <div class="component_deped">
        <img src="./assets/deped-logo.png" alt="DepEd" />
      </div>
      <div class="component_letran">
        <img src="./assets/letran-logo.png" alt="Letran" />
      </div>
    </div>
    <div class="component_text">
      <p>
        Lorem Ipsum is simply dummy text of the printing and typesetting
        industry. Lorem Ipsum has been the industry's standard dummy text ever
        since the 1500s, when an unknown printer took a galley of type and
        scrambled it to make a type specimen book. It has survived not only five
        centuries, but also the leap into electronic typesetting, remaining
        essentially unchanged. It was popularised in the 1960s with the release
        of Letraset sheets containing Lorem Ipsum passages, and more recently
        with desktop publishing software like Aldus PageMaker including versions
        of Lorem Ipsum.
      </p>
    </div>
  </div>
</section>
...
```

<i>CSS</i>

```css
...
.schools{
    display: flex;
    justify-content: center;
    padding-bottom: 100px;
}

.component img{
    width: 150px;
}

.component_container{
    width: 55%;
    border: 6px solid #000;
    border-radius: 50px;
    padding: 100px 80px;
    background-color: #fff;
}

.component{
    display: grid;
    grid-template-columns: 33% 33% 33%;
    grid-template-rows: 1fr;
}

.component_up{
    text-align: left;
}

.component_deped{
    text-align: center;
}

.component_letran{
    text-align: right;
}

.component_text{
    padding: 50px 0px 0px 0px;
}
...
```

---

# The End

<p> Don't worry if some of your approach is not the same on this repository, it doesn't mean that it is wrong. This is just a guide for you on how to make it. </p>
Happy Coding! 🧑‍💻👩‍💻
