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

### Solved Bugs

Being a relatively simple website, I haven't encountered many bugs, but here are the ones I have found.

1. When the clicking on buttons on the nav bar, to go to specific sections of the site, it would cut out the heading of that section, making it look quite askew. This was due to there not being enough padding on the page headings, so they'd cut off when navigating to them.

2. The videos would initially be askew when trying to put them next eachother. After testing this, I found it was easier to put them in seperate columns, and having them one above the other. This also works better for smaller devices, as they are already in layout more suitable to those smaller screens.

3. When I added the images to a carousel, the images would change the shape and size of the carousel, depending on the orignal size of the image. I initially thought that have the carousel in a column class div would be enough to remedy this, but as it's responsive, that wasn't the case at all, quite the opposite. After trying a few different things with the HTML thinking I'd have to resize all of the images, I realised I was overthinking the issue, and just set the max-height for the carousel images in CSS.

### Known Bugs

1. In the image carousel, there a few images that have a smaller max-height than the set 600px. This causes an issue with the carousel shrinking ever so slightly to fit these images. This will be an easy enough fix of just finding the lowest max-height of the images in the carousel and adjusting the max-height in CSS. This will be changed when time permits.