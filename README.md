# Surfboard Volume Predictor

This project is a simple web application for estimating the volume of a surfboard based on its dimensions: height, width, and thickness.

[Surfboard Volume Calculator Link](https://localastronaut.github.io/Surfboard-Volume-Calculator/)



## Overview

The application is a single HTML page that includes a form for entering the dimensions of a surfboard and a JavaScript function that calculates the estimated volume using a linear regression model. The form includes dropdown lists for the height (in feet and inches), width, and thickness (in inches, with quarter-inch increments).

When the user clicks the "Calculate" button, the `calculateVolume` JavaScript function is called. This function retrieves the selected dimensions from the form, calculates the total height in inches, and then uses the linear regression equation to estimate the volume. The estimated volume is then displayed on the webpage.

## Tech Stack

The application is built entirely with HTML, CSS, and JavaScript:

- HTML5: structure of the webpage
- CSS (Bootstrap 4): styling of the webpage
- JavaScript: functionality to calculate and display the estimated volume

## How to Use

1. Open the `index.html` file in a web browser. You should see a form for entering the dimensions of a surfboard.
2. Use the dropdown lists to select the height, width, and thickness of the surfboard.
3. Click the "Calculate" button. The estimated volume will be displayed on the webpage.

## Limitations

The volume estimation is based on a simplified linear regression model, which may not accurately reflect the actual volume of a surfboard, especially for surfboards with unusual dimensions. The model was trained with a small dataset of surfboard dimensions and volumes, so it might not generalize well to other surfboards. The actual volume of a surfboard can be influenced by many factors, including the shape of the surfboard, which is not taken into account by this model.

## Future Work

- Improve the volume estimation model, e.g., by using a more sophisticated machine learning model or incorporating additional features like the shape of the surfboard.
- Add error handling for the form inputs to ensure that the entered dimensions are valid.
- Make the UI more user-friendly, e.g., by adding tooltips to explain what each field is for.
