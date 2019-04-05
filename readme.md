# Vue Training Exercises

## Passing data between components

### Requirements
As a user, I want to be able to update my email address so that the business knows where to contact me.

### Acceptance Criteria
* User is able to enter their email address and submit it
* After submitting a valid email address, the user should be shown a confirmation 
  * Use the Thanks component for the confirmation
* Only one view is visible at a time
  * Ensure that the directive you use to display this component is the _best_ option 
* Running the app produces no errors (in the console or in the terminal)

### Implementation Details
* Update all placeholders (they look like this: %%placeholder%%) with actual values 
  * I.e., if the placeholder is `%%email%%`, replace that with the correct value for the user's email address
* Submitting the user's email address should update the _app's_ data such that other components (`Thanks.vue`) show the _updated_ email address
  * I.e., the Thanks component should get it's data from the parent component, `App.vue`

### Challenge
* If the user's email address did not change (i.e., user provided their current email to the EmailUpdate component), show the user the Thanks component with a conditional message:
  * If the user's email address changed, show the copy, "You updated your email to %%email%%." 
  * If the user's email address did not change, show the copy, "You provided the same email address (%%email%%) that you were already registered with."
* Refactor the method, `onUserUpdate` in `App.vue` to use the spread operator (not Object.assign)