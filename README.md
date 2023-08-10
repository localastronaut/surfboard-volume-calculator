# Surfboard Volume Predictor

This project is a simple web application for estimating the volume of a surfboard based on its dimensions: height, width, and thickness.



## Overview

The application is a single HTML page that includes a form for entering the dimensions of a surfboard and a JavaScript function that calculates the estimated volume using a linear regression model. The form includes dropdown lists for the height (in feet and inches), width, and thickness (in inches, with quarter-inch increments).

When the user clicks the "Calculate" button, the `calculateVolume` JavaScript function is called. This function retrieves the selected dimensions from the form, calculates the total height in inches, and then uses the linear regression equation to estimate the volume. The estimated volume is then displayed on the webpage.

## Tech Stack

The application is built entirely with HTML, CSS, and JavaScript:

- HTML5: structure of the webpage
- CSS (Bootstrap 4): styling of the webpage
- JavaScript: functionality to calculate and display the estimated volume

## Linear Regression Model

The application calculates the volume of a surfboard based on the height, width, and thickness of the surfboard. The volume is calculated using a formula:

volume = 0.69 * height - 0.99 * width + 22.05 * thickness - 54.23

This formula is a representation of a multi-variable linear regression model. In linear regression, we try to model the relationship between two or more features and a response by fitting a linear equation to observed data. Here, the features are the dimensions of the surfboard (height, width, thickness), and the response is the volume of the surfboard.

Here's how each part of the formula corresponds to a component of a linear regression model:

- The values 0.69, -0.99, and 22.05 are the coefficients of the independent variables (height, width, thickness). These coefficients determine the effect of each dimension on the volume of the surfboard.
- The constant term -54.23 is the y-intercept of the model. It represents the value of the dependent variable (volume) when all the independent variables are 0.

The model assumes that the relationship between each dimension and the volume is linear, and the coefficients and constant term are presumably determined through a process of training a linear regression model on a set of data where the dimensions and volumes of various surfboards are known. However, in this application, the model is static and does not update or learn from new data over time.



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
