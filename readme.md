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

### Inspire from 10+ Hamburger menu example [hamburger menu](https://alvarotrigo.com/blog/hamburger-menu-css/)

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

![about me](/docs/mobile-aboutme1.jpg)

Using Floating method to create different layout for each section.

# third page - blog.html

![blogs](/docs/mobile-blog1.jpg)

Using the flexbox layout.

### **And decide the font style for the whole project**

- Noto+Sans
- Lora

# Contact page

![contact me](/docs/mobile-contact1.jpg)

Only Landing image and contact form

```html
    <!-- create a form to submit the contact info -->
    <div class="contact-container">
        <form action="action_page.php">
            <label for="fname">First Name</label>
            <input type="text" id="fname" name="firstname" placeholder="Your first name...">
            <label for="lname">Last Name</label>
            <input type="text" id="lname" name="lastname" placeholder="Your last name...">
            <label for="email">Email</label>
            <input type="text" id="email" name="email" placeholder="Sample: john@gmail.com">
            <label for="message">Message</label>
            <textarea name="message" id="message" placeholder="Wtire something..."></textarea>
            <input type="submit" value="Send">
        </form>
        <div class="side-pic"></div>
    </div>
```

Leave the space for side picture when using desktop and tablet.

# Create the tablet and desktop version

![desktop and tablet1](/docs/desktop-index.jpg)

Nav bar will appear on the top on desktop and tablet version.

![desktop and tablet2](/docs/desktop-index2.jpg)

Only shows the date and title of each blog, you can click the <mark>image</mark> or <mark>explore</mark> at the bottom to go to the blog page. Each blog has an unique ID, so the link will direct you to that blog in stead of the top of blog page.

```html
<div class="blog-item">
    <a href="/pages/blog.html#Blog1"><img src="/pic/blog2-img.png" /></a>
    <div class="blog-date">27 Octorber 2022</div>
    <!-- jump to the specific part of the blog page using id attribute -->
    <h3>Calling all emerging talent: Creative Futures awards competition open for entries</h3>
    <p><a href="/pages/blog.html#Blog1">EXPLORE &#8594</a></p>
</div>
 ```

the <mark>explore -></mark> is an animation link move from left to right

```css
/* create an animation for each artcical's link */
.blog-item p a:hover{
  animation-name: move-right;
  animation-duration: 20s;
}

@keyframes move-right {
  0%   {left:0px; top:0px;}
  100%  {left:400px; top:0px;}
}
```

# Create about page on desktop and tablet

![About page](/docs/desktop-about.jpg)

Make the footer stick to the bottom of the page.

```css
/* set footer fixed to the bottom of the page */
footer{
  position: fixed;
  bottom: 0;
  padding: 15px 0;
  background-color: #36454F;
  color: white;
  text-align: center;
  font-size: 0.7rem;
  width: 100%;
  max-width: 1024px;
}
```

# Create the blog page for desktop and tablet version

![blog page](/docs/desktop-blog.jpg)

Cause the blog container is set as flexbox layout, when the sceen size become bigger, there will be two columns for the blogs. And each blog item has date, title, image and the content with black box shadow.

# Create the contact page for desktop and tablet version

![contact desktop](/docs/desktop-contact.jpg)

The side picture hidded on mobile version, but shows on the desktop version



# Deploy on Netlify

Here is the link ->  [https://lucent-figolla-a402f3.netlify.app/](https://lucent-figolla-a402f3.netlify.app/)

## Reference
- https://unsplash.com/photos/em5w9_xj3uU

- https://www.altamira.ai/blog/common-screen-sizes-for-responsive-web-design/

- https://alvarotrigo.com/blog/hamburger-menu-css/

- https://www.dreamstime.com/stock-illustration-top-view-busy-businessman-working-hard-his-desk-office-lot-paper-work-business-conceptual-image77376239

- https://www.thedrum.com/opinion/2022/10/28/rust-programming-language-the-future-web-development

- https://www.thedrum.com/news/2022/10/27/calling-all-emerging-talent-creative-futures-awards-competition-open-entries

- https://www.techbusinessnews.com.au/news/google-starts-get-the-message-campaign-pressuring-apple-into-rcs-on-the-iphone/
















