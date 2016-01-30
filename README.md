# Web Design with Weebly

## Introductions
- Elise Kain

## Things to Consider
- What is the purpose of this website?
- Who is our primary target audience? Do we have a secondary audience? Who else might visit our website?
- What is the most important information to share?
- What can we do to make our visitors come back and visit the page again?
- What devices/browsers will our visitors be using? Is our site responsive to different screen sizes?
- What can we do to convey a consistent "brand"?

## Web Design Quick Tips
- Create a visual hierarchy
  - Biggest text: most important information
  - Bolded text: this information is more important than regular text
  - Italic text: adds emphasis
- Start with only 1 or 2 fonts
  - Any text using a script font (looks like cursive) should be large and easily readable
  - Make sure there is high contrast between the background and the text
- Create a color palette using only a few colors (&lt;5) as a guideline.
- Design rules are meant to be broken. Just make sure it's for a good reason!

## Weebly Account Setup
- [Sign up](http://www.weebly.com/signup) for a Weebly account.
- Select a theme
- Create a subdomain (like http://turtleretreat.weebly.com)

## Basic Page Customization
- Customize header
- Homepage: Write a header, tag line, and call to action button.
- About Us: Provide a brief history about the organization.
- Contact Us: How to get in touch with the organization.
- Switch to Mobile View from the top navigation to preview the site on mobile devices.

## Add &amp; Edit an Image
- Use Weebly to search for free images (image attribution is automatically added).
- Use [Pixabay](https://pixabay.com/) to search for free images (image attribution is not required).
  - Consider image size needed
  - Download image to computer
  - Upload image to Weebly site

## Add a New Page
- Create a "Get Involved" page
  - Select "Pages" from the top navigation bar.
  - Click the plus sign at the top of the left sidebar menu.
  - Choose to add a "Standard" page
  - Name it "Get Involved"
  - Click "Save"
- Other page customizations
  - Drag the pages around if you'd like to change their order of appearance in the menu.
  - Experiment with different header types, depending on the type of information on each page.
- Create a link to the new page
  - On the homepage, link the "Get Involved" call to action button to the new "Get Involved" page.
  - Click on the button and then select "Link".
  - Select "Standard Page" and then select "Get Involved" from the drop down menu.

## Publish the Site
- Click on "Publish" on the right side of the top navigation.
- Verify your subdomain and that you are not a robot.
- Test out your website in different browsers and with different devices.

## Add custom CSS
- Click on "Theme" in the top navigation.
- Select "Edit HTML/CSS".
- Edit `main_style.css`. You can edit the styles "inline" or add new custom styles at the bottom of the page.
- Save the edited stylesheet as a new template.

```css
/* Original Styles */
.dusk-header .nav-wrap {
  background: #07342a;
}

.nav li#active > a.wsite-menu-item,
.nav li > a.wsite-menu-item:hover {
  background: #052b22;
}

/* Custom Styles */
.dusk-header .nav-wrap {
  background: #7e7e7e;
}

.nav li#active > a.wsite-menu-item,
.nav li > a.wsite-menu-item:hover {
  background: #585858;
}
```

### Help locating CSS styles (with Safari or Google Chrome)
- May need to reference [Safari Developer Tools](http://debugbrowser.com/#safari) or [Chrome Developer Tools](http://debugbrowser.com/#chrome) to set up if you've never used developer tools before.
- In the live site, right click on the element you want to style and select "Inspect" or "Inspect Element". This will open Developer Tools.
- Check out the CSS selectors being targeted in the "Styles" tab.
- Play around by editing CSS properties here and see how they affect the way your website looks.
- Refresh the page to see the original styles applied again.

## Add custom JavaScript/jQuery

- Click on "Theme" in the top navigation.
- Select "Edit HTML/CSS".
- Edit `custom.js`.
- We're going to be adding "event listeners", so we want all our code to stay within the `$(document).ready(function(){})` at the bottom of the file.

```javascript
$(".wsite-button-inner").click(function(){
  alert("Button clicked!");
});
```

- Click save, then publish the updated site. Now, every time a button is clicked on the website, we get the alert box with "Button clicked!".
- While this isn't exceptionally useful by itself, you can expand upon this with modal windows and other more complex actions as you learn more JavaScript or jQuery.

## Helpful Links

### Learn about HTML, CSS &amp; JavaScript
- [CSS Tricks Almanac](https://css-tricks.com/almanac/)
- [w3schools](http://www.w3schools.com/)

### Stock Photos (in the public domain)
- [Pixabay](https://pixabay.com/)
- [MorgueFile](http://www.morguefile.com/)
- [Subtle Patterns](http://subtlepatterns.com/)

### Color Palette
- [Coolors.co](https://coolors.co/app)
- [flatuicolorpicker](http://www.flatuicolorpicker.com/)
- [ColorHexa](http://www.colorhexa.com/)

### Icons and Logo Creation
- [Icomoon.io](https://icomoon.io/app/#/select)
- [Canva](https://www.canva.com/)
- [FontAwesome](https://fortawesome.github.io/Font-Awesome/)

### Lorem Ipsum Generators
- [Cupcake Ipsum](http://www.cupcakeipsum.com/)
- [Minions Ipsum](http://www.minionsipsum.com/)
- [Cheese Ipsum](http://www.cheeseipsum.co.uk/)
- [Harry Potter Ipsum](http://www.christinachern.com/hpipsum/)
