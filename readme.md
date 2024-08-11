  

#  Simple NavBar with accordion effect
Lets make a simple and responsive Navbar template.

##  Branches dev1 and dev2

In these branches the code is split in two parts, the HTML one which was developed on the dev1 branch and the style on the dev2 branch.

##  Branches joint, QA and Main

These Branches were merged and here is the expected outcome:

![screenshot](pics/screenshot1.png)

![screenshot](pics/screenshot2.png)

![screenshot](pics/screenshot3.png)


#  Code analysis
 
##  HTML File

###  Summary:
This creates a navigation bar estructure with a hamburger menu icon, which displays the menues when is clicked.

###  Code:
We start defining a navigation bar with a class of **"navbar"**, which contains a **div** element with a class of **"navbar-overlay"** that, when clicked, calls the **toggleMenuOpen() JavaScript function**.

This overlay is likely used to provide a clickable area for opening or closing a menu.

It continues with the class **"navbar-burger"**. When this button is clicked, it triggers the **JavaScript function "toggleMenuOpen()"**.

Inside the button, there is a **span** element with the class **"material-icons"** that displays the menu icon.

It continues defining a navigation menu, which contains five buttons, each representing a different section of the website.

The **navbar-menu class** is used to style the entire navigation menu, and the **active class** is used to indicate that each button is currently active.

##  CSS File
###  Code:
-  **Importing Google family  font**
>
```
	@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&display=swap');
```

> This line imports the Poppins font from Google Fonts. The **@import** rule is used to include external stylesheets. In this case, the stylesheet is hosted on Google Fonts and the font being imported is Poppins with different weights (300, 400, 500, 600). The **url() function** is used to specify the location of the external stylesheet.
***

-  **Defining Box model**
>
    ```css
	*{
		box-sizing:  border-box;
	}
    ```

> This sets the box model used by the browser to calculate the width and height of elements.
***

-  **Setting the style for all buttons**
>
	```css
	button{
	}
	```
> This rule sets the default styles for all button elements on the page. It sets the border to 0, padding to 0, font family to inherit (the same as the parent element), background to transparent, color to inherit (the same as the parent element), cursor to pointer (indicating that the element is clickable), and sets the font size to 20 pixels.
***

-  **Style for the navigation bar**
>
	```css
	.navbar{
	}
	```
> This defines the styling for the navigation bar.
> 
> Here are the key properties being set:
>  **position:** fixed; means the navigation bar will stay in the same position even when the user scrolls. 
>  **z-index:** 1; sets the stacking order of the element. 
>  **top:** 0; and left: 0; position the navigation bar at the top left corner of the viewport. 
>  **display:** flex; makes the navigation bar a flex container. 
>  **align-items: center; and justify-content:** center; center the content of the navigation bar both vertically and horizontally. 
>  **width: 100%; and height: 80px;** set the width and height of the navigation bar. 
>  **background: #101044;** sets the background color of the navigation bar to a dark blue. 
>  **color: #ffffff;** sets the text color of the navigation bar to white.
>  **font-family: 'Poppins';** sets the font family of the navigation bar to 'Poppins'.
***

-  **Covering NavBar technique**
>
	```css
	.navbar-overlay{
	}
	```
> This technique defines the styling for an element with the class name **navbar-overlay**. It sets the position to fixed, which means the element will stay in the same position even when the page is scrolled. The **z-index** is set to 2, which determines the stacking order of elements on the page. The top and left properties are set to 0, which positions the element at the top left corner of the **viewport**. The **width and height** are set to 100%, making the element cover the entire viewport. The background color is set to a semi-transparent black using the **rgba() function**. The visibility and opacity properties are initially set to hidden and 0, respectively, which means the element is not visible. Finally, the **transition property** is set to 0.5s, which specifies that any changes to the visibility and opacity properties will transition over a duration of 0.5 seconds.
***

-  **Setting visibility properties to overlay**
>
    ```css
	body.open .navbar-overlay{
	}
    ```
> Here we the visibility and opacity properties for the element with the class **navbar-overlay** when the body has a class of "open". This would typically make the navbar-overlay **visible** and fully opaque when the body is in the "open" state.
***

-  **Burguer class**
>
	```css
	.navbar-burger{
	```

> This CSS code snippet defines a class named .navbar-burger. It sets the position of the element to be absolutely positioned at the top left corner of its containing element. It uses a grid layout to center its content. The element has a width and height of 64 pixels, and its padding is set to 0.
***

-  **Styling navigation menu**
>
	```css
	.navbar-menu{
	}
	```

> This defines the style for a navigation menu. The menu will be positioned at the top left corner of the screen, with a width of 270 pixels and a height of 100% of its parent element's height. It will have a padding of 30 pixels, and the content will be displayed in a column with a gap of 10 pixels between each item. The background color will be black, and the menu will be initially hidden. There will be a transition effect of 0.5 seconds for all properties.
***

-  **Setting the style for the button inside the navigation menu**
>
	```css
	.navbar-menu > button{
	}
	```
> This styles the buttons inside the .navbar-menu class. It sets the text color to semi-transparent white, background to transparent, padding around the button text, a transition effect for all properties over 0.3 seconds, and a font size of 17 pixels.
***

-  **@media only screen and (min-width: 600px){**
>
	```css
	@media only screen and (min-width: 600px){
	}
	```
> Here we uses media query to apply specific styles when the screen width is at least 600 pixels.

***

![reading...](https://media.giphy.com/media/Tf3mp01bfrrUc/giphy.gif?cid=ecf05e47wajghtrc5targr7mju7coe0avdyurnehrr1krgdt&ep=v1_gifs_search&rid=giphy.gif&ct=g "...How could I ever do so unless someone guide me?")

***
