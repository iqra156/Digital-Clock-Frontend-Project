# Digital-Clock-Frontend-Project

This project creates a digital clock that dynamically displays the current time, updating every second. The clock is styled with a visually appealing gradient background and a blur effect, making it look modern and sleek. The project consists of three main components:

# HTML (Structure)
CSS (Styling & Layout)
JavaScript (Functionality & Time Updates)
Step 1: Setting Up the HTML Structure
The HTML file provides the basic structure of the web page and includes:

# A container that acts as the main wrapper for the entire page. It takes up the full viewport height.
A centered clock inside a div class="container", which will display the time in HH:MM:SS format.
Three <span> elements that separately display hours (#hrs), minutes (#min), and seconds (#sec). These spans are dynamically updated using JavaScript.
A link to an external CSS file (style.css) for styling.
A script file (script.js) linked at the end of the body to handle the clock's functionality.
Step 2: Designing the Clock with CSS
The CSS file enhances the visual presentation of the digital clock. It includes:

# Background & Color Theme
The entire page has a gradient background that transitions between two shades of purple (#08001f and #30197d), giving it a futuristic look.
The text color is set to white (#fff) for contrast and better visibility.
Positioning & Layout

The clock container (.container) is positioned at the center of the page using transform: translate(-50%, -50%).
A blurry background effect is applied to the clock using backdrop-filter: blur(40px), giving it a stylish glass-like appearance.
Typography & Styling of Time Display

The clock digits are displayed in a large, bold font (80px).
Each time unit (HH, MM, SS) is placed inside a <span> with equal width for alignment.
A small label ("HOURS", "MINS", "SEC") is displayed below each number using the ::after pseudo-element.

# Decorative Elements
Two floating shapes (a square and a circle) are added behind the clock using the ::before and ::after pseudo-elements to enhance aesthetics.
A pink square (#f41b75) is positioned at the top-left.
A blue circle (#419aff) is positioned at the bottom-right.
Step 3: Making the Clock Functional with JavaScript
The JavaScript file (script.js) dynamically updates the time every second.

# Fetching Elements
It first selects the three <span> elements by their IDs (#hrs, #min, #sec) and stores them in variables (hrs, min, sec).
Updating the Time Every Second
A setInterval() function is used to execute the time update every 1000 milliseconds (1 second).
Getting the Current Time
Inside the setInterval(), JavaScript’s Date() object fetches the current hours, minutes, and seconds.
Formatting the Time Display
If a number is less than 10, a leading zero is added (e.g., 09 instead of 9) for a uniform two-digit display.
The updated values are inserted into the respective <span> elements (#hrs, #min, #sec).
