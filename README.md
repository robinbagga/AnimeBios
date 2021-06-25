# Itachi Uchiha Front-End Application
## Demonstrating use of HTML, CSS and Javascript
---
If you've had the chance to look through my GitHub you might have noticed that I truly enjoy being a part of the anime community. So in order to demonstrate web fundamentals and my design skills, I took it upon myself to create a bio page of one of my favorite characters from the hit manga and anime Naruto, Itachi Uchiha.

I truly enjoyed the process of designing the site from the get go and I believe this is going to be a project I will continue to work on and add onto. I began by creating a nice container to fit all the contents of the site into a nice box and tossed in boostrap as well so I could work quicker with the design of the site. I have added everything from images and a YouTube video to a background gradient for the overall site and even Javascript code for a few on-hover elements!

## *Manipulating an image to move on hover*

#### HTML
```
    <div class="wrap-image">
        <img src=https://www.tvovermind.com/wp-content/uploads/2018/07/Itachi-Uchiha.jpg width=70% alt="">
    </div>
```
#### CSS
```
    .wrap-image {
        position: relative;
        max-width: 750px;
        padding-left: 20px;
    }
    .wrap-image::before, .wrap-image::after {
        content: "";
        width: 100%;
        height: 100%;
        position: absolute;
        z-index: -1;
        border: 2px solid black;
        transition: all 0.25s ease-out;
    }
    .wrap-image::before {
        background-color: black;
        top: -15px;
        left: -15px;
        padding-left: 40px;
    }
    .wrap-image::after {
        bottom: -15px;
        right: -15px;
    }
    .wrap-image:hover::before {
        top: 15px;
        left: 15px;
    }
    .wrap-image:hover::after {
        bottom: 15px;
        right: 15px;
    }
```


