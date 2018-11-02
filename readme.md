# Vue Training Exercises

## Mortgage Calculator

### Requirements
As a potential homebuyer, I want to know what my monthly payment will be so that I can ensure I am able to afford the home.

#### Acceptance Criteria
* The user is able to see their mortgage details.
* Calculation is made using the formula: 
  * M = ( P ( 1 + (r/12) )<sup>Y</sup>(r/12) ) / ( (1 + (r/12) )<sup>Y</sup> - 1 )
  where 
    * M = monthly payment
    * r = the loan interest rate expressed as a decimal
      * we divide r by 12 to get a _monthly_ rate
    * P = principle (amount borrowed from the bank)
    * Y = term (in months; i.e, 360 months = 30 years)
  * Formula was taken from [this website](https://www.mtgprofessor.com/formulas.htm) - please use it as a reference.

#### Implementation Details
* __You may not use a button to submit your form__
  * The calculator should update all values instantly without a form submission
  * Updating any field should update the rest of the fields' values
    * User cannot update payment field (it is purely a calculation)

#### Challenge
_If you finish quickly_
* Auto-format the user's rate and mortgage amount
  * Example: inputting '462' will output '4.62%'
  * Example: inputting '100000' will output '$100,000'

OR

* Provide a dropdown menu for term using the following values (in years)
  * 10, 15, 20, 25, 30

OR

* Add a variable rate feature
  * I.e., the rate of the loan will change over time
