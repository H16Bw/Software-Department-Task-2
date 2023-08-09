# Software-Department-Task-2
2nd task of Software Department - Summer training program at Smart Methods

Creates a webpage featuring a control panel to control a robot's

![image](https://github.com/H16Bw/Software-Department-Task-2/assets/139852537/33c4dfa5-9557-4e41-8d6e-6b7d4965265f)


This code creates a webpage featuring a control panel to control a robot's movement and display its motion paths using HTML, CSS, and JavaScript. It defines the structure of the webpage in HTML, specifies the styling of elements in CSS, and manages the robot's movement and path display in JavaScript.

## The main points for each section are as follows:

### HTML (index.html):
- This part of the code defines the webpage's structure using HTML elements.
- <button> elements with unique IDs represent control buttons for moving the robot in different directions (up, down, left, right).
- The <div id="robot"> element represents the display area for the robot.
- The <canvas id="plot"> element is utilized to draw and exhibit the robot's movement path.
- The <script> tag at the bottom refers to an external JavaScript file (script.js) responsible for handling robot movement and path display.

### CSS (style.css):
- This section establishes the styles and layout for webpage elements.
- Body styles define margins, spacing, and font for the entire document.
- Styles for #controls position the control panel on the left side of the screen using absolute positioning and vertical alignment.
- Styles for #controls button define the appearance of the control buttons, including background color, font size, and border radius.
- Styles for #robot position the robot at the center of the screen using absolute positioning and both vertical and horizontal alignment.
- Styles for #plot position the canvas element to cover the entire webpage and set a background color.

### JavaScript (script.js):
- This section manages the robot's movement and path display using JavaScript.
- It starts by selecting the robot element and the canvas element using their respective IDs.
- The pathData array is initialized to store coordinates of the robot's movement.
- The moveRobot() function is defined to control the robot's movement:
  - It accepts a direction parameter (up, down, left, right).
  - Depending on the direction, it updates the robot's position (top and left CSS properties) and adds new coordinates to the pathData array.
  - Then, it clears the canvas, starts a new path, and draws the path using coordinates stored in the pathData array.
  - Event listeners are added to each button using addEventListener() to listen for button click events.
  - When a button is clicked, the corresponding direction is passed to the moveRobot() function.
