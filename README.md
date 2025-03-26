Clarification Questions


1 -If the user does not reset the password soon, is it possible to resend it, or does the process need to be restarted?

2-What happens if the account creation process takes more than 3 seconds?

3-Should the system check if the email is already registered?

4-Should duplicates be identified based on the registered name?



Test Cases


Test Case 1 - Temporary Password Email

Description: Verify if the user receives an email with the temporary password after account creation.
Steps:

-Create a new account.

-Check the registered email for a message containing the temporary password.

Expected Result:
The user should receive an email with the temporary password shortly after account creation.


Test Case 2 - Prolonged Creation Process

Description: Check what happens if the account creation process takes more than 3 seconds.

Steps:
-Attempt to create a new account with a delay exceeding 3 seconds.
-Observe what happens when the process takes too long.

Expected Result:
The system should either complete the process within the expected time or prompt the user to restart the process.




Test Case 3 - Email Already Registered

Description: Verify if the system prevents account creation with an already registered email.

Steps:

-Try to create an account using an email that is already registered.

Expected Result:
The system should prevent account creation and inform the user that the email is already in use.


Test Case 4 - Mandatory Fields

Description: Check if it is possible to create an account without providing a required field (e.g., last name).

Steps:

-Attempt to create an account using only an email and first name, leaving the last name field blank.

Expected Result:
The system should notify the user that all mandatory fields must be filled in before proceeding.


Test Case 5 - Field Size Limits

Description: Verify if the system enforces character limits on input fields.

Steps:

-Try to create an account using:

An email longer than 30 characters.

A first name longer than 10 characters.

A last name longer than 12 characters.

Check if the system allows the user to proceed.

Expected Result:
The system should prevent account creation and inform the user that the character limits have been exceeded.
