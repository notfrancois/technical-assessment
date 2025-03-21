# Frontend Form Exercise: Contact Us Form

## Overview

Building forms is a common task in Front End. In this exercise, we will build a basic "Contact Us" form, commonly seen on marketing websites for visitors to ask questions or provide feedback.

## Requirements

The form should contain the following elements:

-   Name field.
-   Email field.
-   Message field. Since the message can be long, a `<textarea>` will be more suitable.
-   Submit button
-   Contains the text "Send".
-   Use a `form` element to wrap the form fields and the submit button.
-   You can apply any styles you want to the form fields and the submit button. (You can use CSS or Tailwind CSS)

Clicking on the submit button submits the form.

> Please note that the form and submission **SHOULD** be implemented entirely in HTML. Do not use any JavaScript or framework-specific features for this question.

There is no need to do any client-side validation on the fields. Validation will be done on the server side.

## Submission API

Upon submission, POST the form data to https://www.greatfrontend.com/api/questions/contact-form with the following fields in the request body: name, email, message.

If all the form fields are correctly filled up, you will see an alert containing a success message. Congratulations!

## Notes

You do not need JavaScript for this question, the focus is on HTML form validation and submission.
