
# Simple NavBar
Lets make a simple and responsive Navbar template.


## Branches dev1 and dev2
In these branches the code is split in two parts, the HTML one which was developed on the dev1 branch and the style on the dev2 branch.

## Branches joint, QA and Main
These Branches were merged and will look as follow:

![screenshot](pics/screenshot1.png)

![screenshot](pics/screenshot2.png)
![screenshot](pics/screenshot3.png)

# Code analysis

## HTML File

### Summary:
This creates a navigation bar estructure with a hamburger menu icon, which displays the menues when is clicked.

### Code:
We start defining a navigation bar with a class of **"navbar"**, which contains a **div** element with a class of **"navbar-overlay"** that, when clicked, calls the **toggleMenuOpen() JavaScript function**. 
This overlay is likely used to provide a clickable area for opening or closing a menu.

It continues with the class **"navbar-burger"**. 
When this button is clicked, it triggers the **JavaScript function "toggleMenuOpen()"**. 
Inside the button, there is a **span** element with the class **"material-icons"** that displays the menu icon.

It continues defining a navigation menu, which contains five buttons, each representing a different section of the website.
The **navbar-menu class** is used to style the entire navigation menu, and the **active class** is used to indicate that each button is currently active.


## CSS File

### Code:

- **@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&display=swap');** 
>> This line imports the Poppins font from Google Fonts. The **@import** rule is used to include external stylesheets. In this case, the stylesheet is hosted on Google Fonts and the font being imported is Poppins with different weights (300, 400, 500, 600). The **url() function** is used to specify the location of the external stylesheet.


- **box-sizing: border-box;**
 >> This sets the box model used by the browser to calculate the width and height of elements.

- **button{**
>> This rule sets the default styles for all button elements on the page. It sets the border to 0, padding to 0, font family to inherit (the same as the parent element), background to transparent, color to inherit (the same as the parent element), cursor to pointer (indicating that the element is clickable), and sets the font size to 20 pixels
 

- **.navbar{**
>> Defines the styling for a navigation bar (.navbar).

Here are the key properties being set:

position: fixed; means the navigation bar will stay in the same position even when the user scrolls.
z-index: 1; sets the stacking order of the element.
top: 0; and left: 0; position the navigation bar at the top left corner of the viewport.
display: flex; makes the navigation bar a flex container.
align-items: center; and justify-content: center; center the content of the navigation bar both vertically and horizontally.
width: 100%; and height: 80px; set the width and height of the navigation bar.
background: #101044; sets the background color of the navigation bar to a dark blue.
color: #ffffff; sets the text color of the navigation bar to white.
font-family: 'Poppins'; sets the font family of the navigation bar to 'Poppins'.