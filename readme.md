
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

This creates a navigation bar with a hamburger menu icon, which display the menues when is clicked.


We start defining a navigation bar (<nav>) with a class of "navbar". It contains a <div> element with a class of **"navbar-overlay"** that, when clicked, calls the **toggleMenuOpen() JavaScript function**. 
This overlay is likely used to provide a clickable area for opening or closing a menu.

It continues with with the class **"navbar-burger"**. When this button is clicked, it triggers the **JavaScript function "toggleMenuOpen()"**. 
Inside the button, there is a span element with the class **"material-icons"** that displays the menu icon.

It continues defining a navigation menu, which contains five buttons, each representing a different section of the website.
The **navbar-menu class** is used to style the entire navigation menu, and the **active class** is used to indicate that each button is currently active.


## CSS File