# Calculator
I have made a calculator for my Internship at Lets Grow More Community in HTML, CSS and JS
https://tanvicalculator.netlify.app/
The first line selects an HTML element with the ID "inputBox" and assigns it to the variable input. This element is typically an input or textarea where the calculator's display or input is shown.

The second line selects all the button elements on the page and assigns them to the variable buttons. The querySelectorAll function returns a NodeList, which is similar to an array.

The variables string and arr are initialized. string is used to store the current expression or calculation, and arr is created by converting the buttons NodeList to an array using Array.from().

The code then iterates over each button in the arr array using the forEach() method. For each button, an event listener is added to handle the 'click' event.

Inside the event listener function, the code checks the innerHTML of the clicked button to determine the action to take.

If the button's innerHTML is '=', it means the user wants to evaluate the expression. The eval() function is used to evaluate the string expression, and the result is assigned back to string. The value of the input element is then updated with the result using input.value = string.

If the button's innerHTML is 'AC', it means the user wants to clear the input. In this case, string is reset to an empty string, and the input value is updated accordingly.

If the button's innerHTML is 'DEL', it means the user wants to delete the last character from the input. The substring() function is used to remove the last character from string, and the input value is updated.

If none of the above conditions match, it means the user clicked a digit or an operator button. The innerHTML of the clicked button is appended to the string, and the input value is updated.

By using event listeners and checking the innerHTML of the clicked button, this code allows the user to input mathematical expressions and perform calculations in the calculator interface.
