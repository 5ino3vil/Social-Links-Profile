# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page
- Watch the Latest release.

### Screenshot

![](./SociallinksScreenshot.png)



### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid


**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

When I initially started this project I was unsure on how to place the grey background on the black overall background
My first mistake was setting a background colour for the whole page instead of the body of the page
I then tried to make a container to the main body to add a background colour for the grey background box but this didnt work as the text would have black background on it due to my mistake of adding the background colour to the whole page.
I also initially tried to make the links buttons that were customisable
Then I made them links with background colours and rounded border to imitate a button but realised depending on text the borders would vary in length and were non responsive to the page.
This then promted me to us flex boxes. 
I added flex box collumn to the body for a black background
Nested in the body I then added flex box collumn to the main section - this created the grey background box

I also was making the mistake with the links as making them all seperate flex boxes.
However on doing research realised it was best to make them an unordered list and then make the list a flex box as well!

The added Youtube video was also very hard to intergrate into my main div section. The video edges would come out of the box if i resized the screen.
I also was having issues with the aspect ratio of the embedded video, with the video height being too short compared to the width. it seems that padding bottom in youtube class css fixed this.

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.



```html
   <p>"Your Modern Day Sade"</p><br>
   <div class="Socialbox">
     <ul>
      <li><a target="_blank" href="https://www.instagram.com/5ino3vil" id="insta">Instagram</a></li> 
      <li><a target="_blank" href="https://open.spotify.com/artist/4Zi5nfj3gavmdAxg6NYEmG" id="Spotify">Spotify</a></li> 
      <li><a target="_blank" href="https://www.youtube.com/@5ino3vil" id="youtube">Youtube</a></li>  
      <li><a target="_blank" href="https://music.apple.com/gb/artist/sino-ako/1336015786" id="apple">Apple</a></li>
     </ul><br>  
   </div>  
   <H2 style="color: whitesmoke;">LATEST RELEASE</H2>
   <div class=youtube><iframe 
    width="100%" 
    height="800px" 
    src="https://www.youtube.com/embed/tcn9SOTtJIU?si=RFtic4AKvq1hlv3V" 
    title="Sino Ako - Worn out" frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
    allowfullscreen></iframe></div>
 </main><br>
```
```css 
.youtube {
    width: 100%;
    max-width: 100%;
    height: 0;
    padding-bottom: 56.25%;
    position: relative;
    overflow:hidden ;
    margin: 20px;
}

iframe {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0%;
}


body {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
    background-color: #000000;
}

main { 
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    max-height: 60%;
    max-width: 40%;
    background-color: #2e2e2e;
    border-radius: 10px;
    padding: 2%;


### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Resource 1](https://www.shecodes.io/athena/9191-centering-an-unordered-list-with-css-flexbox) - This helped me for understanding how to put a list into flexbox reason. 
- [Resource 2](https://www.chatgpt.com) - This helped me get better questions as well as debug my code to see where i could possibly be going wrong.
- [Resource 3](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - This helped me understand what flex boxes actually were. With really easy to understand breakdowns of it. 



## Author

- Website - [Sino Ako](https://www.instagram.com/5ino3vil)
- Frontend Mentor - [@5ino3vil](https://www.frontendmentor.io/profile/5ino3vil)

## Acknowledgments

ChatGPT - lol
