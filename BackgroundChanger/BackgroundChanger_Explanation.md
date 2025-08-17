# 🎨 Background Color Changer

This project changes the **background color** of the page randomly whenever the button is clicked.  
It is built using **HTML, CSS, and JavaScript.

 🎥 Demo
[Background Changer Demo](BackgroundChanger_Demo.gif)

💻 Code with Explanation


<!DOCTYPE html>  
<!-- Defines the document type as HTML5 -->

<html>  
<!-- Root element of the HTML page -->

<head>  
  <title>Color Changer</title>  
  <!-- Title of the web page, shown on the browser tab -->

  <style>
    body {
      text-align: center;       /* Centers text horizontally */
      padding-top: 100px;       /* Pushes content down by 100px */
      background-color: lightblue; /* Initial background color */
      font-family: Arial; /* Sets clean font style */
    }

    h1 {
      color: darkblue;          /* Heading text color */
    }

    button {
      padding: 15px 30px;       /* Space inside button */
      font-size: 18px;          /* Increases text size */
      background-color: darkblue; /* Button background */
      color: white;             /* Button text color */
      border: none;             /* Removes default border */
      border-radius: 10px;      /* Rounds button corners */
      cursor: pointer;          /* Shows hand cursor on hover */
    }

    button:hover {
      background-color: purple; /* Button color when mouse hovers */
    }
  </style>
</head>

<body>
  <h1>Click the Button to Change Color!</h1>
  <!-- Heading displayed on the page -->

  <button onclick="changeColor()">Change Background</button>
  <!-- Button that calls the 'changeColor()' function on click -->

  <script>
    function changeColor() {
      // Create an array of colors
      let colors = ["lightblue", "lightgreen", "lightpink", "yellow", "orange", "lavender", "peachpuff"];

      // Pick a random color from the array
      let randomColor = colors[Math.floor(Math.random() * colors.length)];

      // Apply the random color to the background of the page
      document.body.style.backgroundColor = randomColor;
    }
  </script>

</body>
</html>
