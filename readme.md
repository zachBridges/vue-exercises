# Vue Training Exercises

## Form Validation

### Requirements
As a user, I want to be guided through filling out a contact form so that I can submit accurate information to the server (in order to be contacted later).

#### Acceptance Criteria
* Submitting an invalid form shows errors 
* No errors should be displayed before form is submitted
  * Errors are not shown initially
* Name field requires at least three characters to be valid
* Email field requires a valid email address 
* Phone number field requires a valid phone number 
  * Phone number must be a minimum of 10 digits


#### Implementation Details
* Write your own validation or use a library
* Any regex validation must be as performant as possible
* Form should not submit to server until form data is valid
* Do your best to have NO linter errors

#### Challenge
_If you finish quickly_
* Combine the email and mobile number fields so that a user can provide *either* an email address *or* phone number
