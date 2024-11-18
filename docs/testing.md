# Mr Johnson - Testing

## Contents

* [Automated Testing](#automated-testing)
    * [W3C](#w3c)
    * [Lighthouse](#lighthouse)
* [Manual Testing](#manual-testing)
    * [Solved Bugs](#solved-bugs)

## Automated Testing

### W3C

[W3C CSS](assets/img/readme/w3c-css.jpg)
[W3C HTML](assets/img/readme/w3c-html.jpg)

### Lighthouse

[Desktop](assets/img/readme/lighthouse-desktop.jpg)
[Mobile](assets/img/readme/lighthouse-mobile.jpg)

The main thing that gave poor results in the Lighthouse test was the best practices. Looking at this, it's third party cookies that are causing the issue.

I also had a problem with the performance when testing it for mobile, it would vary quite regularly. I think  this is mainly down to the age of my laptop, with which I was testing the website.

## Manual Testing

| Goals | How Are They Achieved? |
| :--- | ---: |
| First Time Visitors |
| Understand that the site is for fans of the band Mr Johnson. | The first thing visitors to the website will see is an image of the band and a description of who the band are. |
| Have easy access to contact us | Our email address is fixed at the bottom of the page |
| Have easy access to our social media platforms | The Social media platforms are fixed to the bottom of the page. |
| Be able to hear what the band sounds like | There are videos and audios tracks, which both have a link on the navbar |
| | |
| Returning Visitors |
| Access to new content such as videos and music tracks | Returning visitors should hopefully see how the amount of content increases, and eventually each section has it's own page. |
| See upcoming gig dates | The users can quickly access our upcoming gigs be selecting the button in the navbar or scrolling down to the appropriate section. |
| Access to Spotify | Mr Johnson will soon be on spotify, a link to which will be added to the fixed footer |

| Feature | Expected Outcome | Testing Performed | Result | Pass/Fail |
| --- | --- | --- | --- | --- |
| Site title page | Clicking the button will take the user to the top of the page | Clicked the title page button | User is taken to the Home Page section | Pass |
| Nav buttons | Clicking on the selected nav button will take the user to the desired section | Clicked on all of the nav buttons | All buttons work and take user to desired section | Pass |
| Navbar hover effect | When cursor is over any navbar buttons the colour of the buttons will change, and change back when cursor is moved away | Cursor was hovered over all navbar elements | All navbar buttons changed colour and then changed back when cursor is moved away | Pass |
| YouTube video | When the play button is clicked, it will start the video and all the YouTube controls are available | Play button was pressed | The videos played and all YouTube media control are available | Pass |
| Music player | The user can play, mute, select a specific part of the song and download the track | The songs was played, muted, downloaded and the seeking bar was used to select specific parts of the song | Everthing works as it's supposed to | Pass |
| Gallery Carousel | Images automatically scroll through the gallery without needing user interaction | No action required | Images automatically go through rotation, eventually displaying all images in the gallery | Pass |
| Gallery Buttons | Goes to next or previous image | Both buttons were pressed | Next or previous is displayed, depending on which button is clicked | Pass |
| Scrolling | Using the scrollbar allows users to navigate up and down the page | Clicking and dragging the scrollbar. Using a mouse wheel and touchpad to navigate | The page scrolls up and down as expected | Pass |
| Email button | Will open the users default email option or when right clicked, gives the option to copy email address | Clicked on the email button | When clicked, Gmail is opened. When right clicked, more options are available, including copying email address | Pass |
| Youtube button | The button should take the user to the Mr Johnson YouTube page, opening in a new tab | Clicking on the link | A new tab opens and takes the user to the Mr Johnson YouTube page | Pass |
| Facebook button | The button should take the user to the Mr Johnson Facebook page, opening in a new tab | Clicking on the link | A new tab opens and takes the user to the Mr Johnson Facebook page | Pass |


### Solved Bugs

Being a relatively simple website, I haven't encountered many bugs, but here are the ones I have found.

1. When the clicking on buttons on the nav bar, to go to specific sections of the site, it would cut out the heading of that section, making it look quite askew. This was due to there not being enough padding on the page headings, so they'd cut off when navigating to them.

2. The videos would initially be askew when trying to put them next eachother. After testing this, I found it was easier to put them in seperate columns, and having them one above the other. This also works better for smaller devices, as they are already in layout more suitable to those smaller screens.

3. When I added the images to a carousel, the images would change the shape and size of the carousel, depending on the orignal size of the image. I initially thought that have the carousel in a column class div would be enough to remedy this, but as it's responsive, that wasn't the case at all, quite the opposite. After trying a few different things with the HTML thinking I'd have to resize all of the images, I realised I was overthinking the issue, and just set the max-height for the carousel images in CSS.

### Known Bugs

1. In the image carousel, there a few images that have a smaller max-height than the set 600px. This causes an issue with the carousel shrinking ever so slightly to fit these images. This will be an easy enough fix of just finding the lowest max-height of the images in the carousel and adjusting the max-height in CSS. This will be changed when time permits.

2. When the site is being viewed on a smaller screen, the videos extend past the the the parent div, so the formatting looks a bit off. All content stay within the screen, it just doesn't look great. 