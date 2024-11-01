# Project 3: Around The U.S.

### Overview

- Intro

**Intro**

This project is called Around the U.S. The is responsive, meaning it is made so all the elements are displayed correctly on popular screen sizes. The figma design gives us specific details at 1280px (normal desktop size) and 320px (normal phone size.) I also added my own specific details at 775px (normal tablet size.) I kept the desktop design, decreased the font size on the Title to 36px, and shortended the add button to 100px. This makes the view at 775px just as enjoyable as it is at 1280 px.

There was some discussion about how elements should react while growing and shrinking the screen, but my own opinion is the point is providing a pleasant and useful product to the User at whatever screen size they are viewing. The User is not going to grow and shrink the image on their device.

The User will eventually be able to make there own page. They make the Title their own, describe themselves, and upload their own pictures.

The responsiveness of this project is done using two different techniques. The first one is the use of grid which will determine the number of cards displayed at each viewing size.

.card\_\_list {
display: grid;
justify-content: center;
grid-template-columns: repeat(auto-fit, 282px);
gap: 20px 17px;
padding: 0;
margin: 0;
}

The "repeat" function will give as many cards of 282px as possible for the viewing device. This is what determines three cards for desktop, two cards for tablet, and one card for the phone. The choice of grid works extremely well for items of the same size that repeat. In our case that is the cards.

The second technique is called Media Queries. This works best when unique items need to move in relation to each other. Media Queries means to display items in a designated way depending upon the screen size of the device being used.

Best example here is the profile information section located above the cards. There is one prestation at desktop size. Design is similar, but smaller, at tablet size. Finally, a vertical presentation as opposed to the previous horizontal one.

In the profile file you will find examples:

@media screen and (max-width: 790px) {
.profile\_\_add-button {
width: 100px;
}

and

@media screen and (max-width: 765px) {
.profile {
flex-direction: column;
margin: 0 auto;
}

You can find the project at:

https://goofyfather.github.io/se_project_aroundtheus/

You can find the video descrition of the project at:

https://www.loom.com/share/8dc66639ce5b4fc6a36820b8d0fd9aa7?sid=504bd795-19bf-43d9-b42b-2e85aa38f780

Enjoy.
