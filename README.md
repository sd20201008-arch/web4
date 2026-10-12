Student Name: Sakenov Danial
Group: SE-2540

 Overview
This project demonstrates the implementation of responsive, accessible, and user-friendly web forms using HTML5, Bootstrap 5.3, and custom JavaScript validation logic. It covers basic HTML form controls, advanced Bootstrap styling, layout grid usage, and client-side form validation techniques.

 Key Features

Part 1
Form Controls & Label: Created accessible forms using semantic HTML tags . Linked labels to inputs using matching `for` and `id` attributes to improve accessibility and user click targets.
Task 1:  Utilized built-in HTML5 attributes such as `required`, `type="email"`, and `maxlength="250"` to enforce basic validation at the browser level without writing custom code.
![alt text](<Screenshot 2026-10-12 at 15.54.04.png>)

Part 2
Bootstrap Grid Layout: Applied Bootstrap grid classes to structure input fields responsively across different screen sizes.
Bootstrap Validation: Implemented contextual validation feedback using `.is-valid` and `.is-invalid` classes along with `.valid-feedback` and `.invalid-feedback` text blocks to visually inform users of their input status.
![alt text](<Screenshot 2026-10-12 at 15.54.34.png>)
Part 3
Built a comprehensive user registration form containing a wide range of input types:
   Text & Email: First Name, Last Name, and Email with format validation.
   Password : Includes `minlength="6"` validation and password confirmation fields.
   inline Radio Buttons: Gender selection using `form-check-inline`.
   Inline Checkboxes:Multiple choice selection for Hobbies.
   Select Dropdown: Country selection with a disabled default placeholder option.
   Action Buttons: Submit (`.btn-success`) and Reset (`.btn-secondary`) buttons.

![alt text](<Screenshot 2026-10-12 at 15.54.55.png>)
JavaScript 

To provide a seamless user experience, default browser tooltip alerts were disabled using the `novalidate` attribute on the `<form>` element. 

Custom JavaScript logic was implemented as follows:
1. Targeting Forms: Queries forms marked with the `.needs-validation` class.
2. Event Listener: Intercepts the `submit` event prior to form submission.
3. Validity Check: Uses the native `form.checkValidity()` method to evaluate whether all fields comply with specified HTML constraints .
4. Preventing Default: If validation fails, `event.preventDefault()` stops the form from submitting and refreshing the page.
5. Visual Feedback: Adds the `.was-validated` class to the form, triggering Bootstrap's dynamic green/red feedback borders and helper messages.

![alt text](<Screenshot 2026-10-12 at 15.55.10.png>)
