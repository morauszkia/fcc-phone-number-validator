# Telephone Number Validator

## Task

Objective: Build a Telephone Number Validator app that is functionally similar to https://telephone-number-validator.freecodecamp.rocks
Fulfill the user stories and pass all the tests below to complete this project. Give it your own personal style. Happy Coding!

### US Phone Number Formats

In the US, phone numbers can be formatted in many ways. Here are some examples of valid formats for US phone numbers:

```
1 555-555-5555
1 (555) 555-5555
1(555)555-5555
1 555 555 5555
5555555555
555-555-5555
(555)555-5555
```

The area code is required. Also, if the country code is provided, the country code must be 1.

## User Stories

1. You should have an input element with an id of "user-input"
2. You should have a button element with an id of "check-btn"
3. You should have a button element with an id of "clear-btn"
4. You should have a div, span or p element with an id of "results-div"
5. When you click on the #check-btn element without entering a value into the #user-input element, an alert should appear with the text "Please provide a phone number"
6. When you click on the #clear-btn element, the content within the #results-div element should be removed

## Tests

### Valid numbers

- When the #user-input element contains 1 555-555-5555 and the #check-btn element is clicked, the #results-div element should contain the text "Valid US number: 1 555-555-5555"
- When the #user-input element contains 1 (555) 555-5555 and the #check-btn element is clicked, the #results-div element should contain the text "Valid US number: 1 (555) 555-5555"
- When the #user-input element contains 5555555555 and the #check-btn element is clicked, the #results-div element should contain the text "Valid US number: 5555555555"
- When the #user-input element contains 555-555-5555 and the #check-btn element is clicked, the #results-div element should contain the text `"Valid US number: 555-555-5555"
- When the #user-input element contains (555)555-5555 and the #check-btn element is clicked, the #results-div element should contain the text "Valid US number: (555)555-5555"
- When the #user-input element contains 1(555)555-5555 and the #check-btn element is clicked, the #results-div element should contain the text "Valid US number: 1(555)555-5555"
- When the #user-input element contains 1 555 555 5555 and the #check-btn element is clicked, the #results-div element should contain the text "Valid US number: 1 555 555 5555"
- When the #user-input element contains 1 456 789 4444 and the #check-btn element is clicked, the #results-div element should contain the text "Valid US number: 1 456 789 4444"

### Invalid numbers

- When the #user-input element contains 555-5555 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 555-5555"
- When the #user-input element contains 5555555 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 5555555"
- When the #user-input element contains 1 555)555-5555 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 1 555)555-5555"
- When #user-input contains 123**&!!asdf# and #check-btn is clicked, #results-div should contain the text "Invalid US number: 123**&!!asdf#"
- When the #user-input element contains 55555555 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 55555555"
- When the #user-input element contains (6054756961) and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: (6054756961)"
- When the #user-input element contains 2 (757) 622-7382 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 2 (757) 622-7382"
- When the #user-input element contains 0 (757) 622-7382 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 0 (757) 622-7382"
- When the #user-input element contains -1 (757) 622-7382 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: -1 (757) 622-7382"
- When the #user-input element contains 2 757 622-7382 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 2 757 622-7382"
- When the #user-input element contains 10 (757) 622-7382 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 10 (757) 622-7382"
- When the #user-input element contains 27576227382 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 27576227382"
- When the #user-input element contains (275)76227382 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: (275)76227382"
- When the #user-input element contains 2(757)6227382 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 2(757)6227382"
- When the #user-input element contains 2(757)622-7382 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 2(757)622-7382"
- When the #user-input element contains 555)-555-5555 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 555)-555-5555"
- When the #user-input element contains (555-555-5555 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: (555-555-5555"
- When #user-input contains (555)5(55?)-5555 and #check-btn is clicked, #results-div should contain the text "Invalid US number: (555)5(55?)-5555"
- When the #user-input element contains 55 55-55-555-5 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 55 55-55-555-5"
- When the #user-input element contains 11 555-555-5555 and the #check-btn element is clicked, the #results-div element should contain the text "Invalid US number: 11 555-555-5555"
