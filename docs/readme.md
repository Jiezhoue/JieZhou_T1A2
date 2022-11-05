# Portfolio website built from scratch

- html
- css
- wireframes
- git
- markdown

# First time try to do the bamburger menu, failed.
the example is Javascript.

# Decide the color scheme
![color scheme](/docs/color-palette.jpg)

Fan of the black and white kind of cool color.
Gray scheme decided for the whole portfolio project.



# Do the mockup - layout, content, color, fonts.

Start from the mobile version, the index.html page will include all general content of each sub pages (about, blog and contact).

![mockup of the landing page](/docs/mobile-idea.jpg)

# Create the logo and find the image for landing page

[landing image](https://unsplash.com/photos/em5w9_xj3uU) from **unsplash**

using illustrator create the logo.

# Mockup for mobile version with landing image, logo and some contents

![mobile version](/docs/mobile-layout1.jpg)

<mark>Still want to do the hamburger menu for mobile, cause 99% of the mobile web are using this function.<mark>


# Roughly finish the index.html page on mobile version.
*### The hamburger menu is using checkbox function.*

```html
<!-- create an invisible checkbox for hamburger menu -->
<input type="checkbox" name="checkbox" id="checkbox">
<div class="hamburger-lines">
    <span class="line line1"></span>
    <span class="line line2"></span>
    <span class="line line3"></span>
</div>      
```
```css
  /* make the checkbox at the same position 
  with the hamburger menu and increase the checkbox size */
  .navbar-container input[type="checkbox"] {
      position: absolute;
      display: block;
      height: 32px;
      width: 30px;
      top: 30px;
      right: 30px;
      z-index: 99;
      opacity: 0;
  }
```
the checkbox size will be the same as hamburger menu at the top right corner, and set the <mark>opacity to 0</mark> (invisible), but the <mark>z-index is 99</mark> (on top of every contents of page)


# Start second page - about.html



