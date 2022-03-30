# Calculator
This is a simple calculator functionality achieved using Javascript. The logic is very simple with the minimum lines of code possible.

## Steps to execute this calculator:

Download the entire code


Open up the index.html.





## Technologies used:


HTML


CSS [style/Presentation]


Javascript [Logic/Working of calculator]



# HTML

The html will be pretty simple for this project. We'll start out with a standard HTML5 boilerplate. At the bottom of our body I included the script.js script that we will create later. This needs to be at the bottom, because this way, when our javascript runs, the html elements required for the calculator will be in the DOM.
In the body we have a section and inside that a div with a container class. We will use these wrappers to position our calculator on the page. Inside our container we have an empty div with the id of display, and this will be the display of our calculator. It is empty, because we will modify its content from Javascript. Then we have a div with the class of buttons which will represent the keypad of the calculator.


The buttons container will hold all of the buttons. Each button will be a div with a class of button. This will make the styling easy, and also will help us to gather the user input. Here we have a div for every button that we want on our keypad. You can notice that we have a label between the buttons, this is a HTML entity and it renders a back arrow (←), and we'll use this as a backspace.


And this is all of the HTML markup that we need for this project, let's jump into CSS.

Don't forget to link the CSS styleshead in the head of the HTML file.

# CSS

Let's create a style.css file.
We set a width and height for the container and using margin (also give it a decent margin of 20px), and apply a little box shadow.



For the display we set a fixed height, and to center the text vertically we need to set the line-height to the exact same amount. The text should be right align, because this is how most calculator displays work. Also set the font-size and give a decent amount paddings.



# Javascript

This will be the heart of our application. Let's create the script.js file. The first thing we need to do is to save a reference to our display dom element. We can easily do that because it has an id of display.

Next we have to get references for the buttons. We'll store the button references in an array. To gather the buttons we can select them by document.getElementsByClassName()

The next and last step we have to make is to add event listener to the buttons and build the functionalities. To add event listeners for the buttons, we'll map through the buttons array and add a click event listener for each.
