# Test-Case Sample - Instagram Login Page

Hello,

Below you'll find a brief test case I've designed to test Instagram's login page. I want to mention that the test case **_is not exhaustive_**; it only targets a few functionality tests aimed to verify aspects such as:

+ UI elements
+ Successful Authentication
+ Failed Authentication
+ Non-functional testing

OS: Windows

Current Instagram Login Page at 15.04.2024 

![Screenshot of Instagram Login Page.](https://i.ibb.co/mNXyrVJ/Untitled.jpg)

## 1. Accessing the Login page

**Description:** Verify if the web site address, once accessed, is redirecting the user to the proper login page.

**Steps to reproduce:** 
1. Open any internet browser
2. Insert https://www.instagram.com/ address în the url field and press Enter

**_Expected results:_** The user is redirected to the Instagram Login page

## 2. Verify the presence and location of UI elements 
// UI Elements - presence and appearance

**Description:** Verify if all the intended UI assets are present and well placed when the login page is accessed. 

**_Expected results:_** The following web site elements should be present and placed accordingly when reaching the login page: 

* The Login header which is centered în the middle of the page
* Instagram Logo text inside the login header
* Email and password text field input inside the login header
* “Phone Number, username, or email” placeholder text is present inside the Email field
* “Password” placeholder text is present inside the password field
* The log în button inside the login header
* Alternative log în way via facebook platform which is delimited by “OR” text inside the login header
* The Log în facebook logo followed by “Log în with facebook” hyperlink text inside the login header
* “Forgot Password?” hyperlink text inside the login header
* “You can also report content you believe is unlawful in your country without logging in.” text inside the login header
* “report content you believe is unlawful” is a hyperlink text
* All the login header’s elements follows the aforementioned order and location

* The Sign up header which can be located immediately after the Login header
* The sign up header contains “Don't have an account? Sign up” text 
* “Sign up” is a blue hyperlink bold text

* The sign up header is followed by “Get the app.” text
* “Get the app.” text is followed by both Google play and Microsoft store icons

* On the left side of both login and sign up headers, a mobile version of the platform is showcased by using few în-app mobile screenshots

* Footer section containing the following hyperlinks: Meta, About, Blog, Jobs, Help, API, Privacy, Terms, Locations, Instagram Lite, Threads, Contact Uploading & Non-Users, Meta Verified
* Web Site language selector which is a drop down list button, inside the footer section
* “© 2024 Instagram from Meta” text, inside the footer section

**Steps to reproduce:** 
1. Open any internet browser
2. Access the Instagram Login Page using https://www.instagram.com/ 


## 3. Test the email input field character limit
// Functionality tests

**Description:** Verify the maximum number of characters allowed for the email input field. 

**Steps to reproduce:** 
1. Access the Login page
2. Select the email input field
3. Insert more than 75 characters 

**_Expected results:_** The user is not able to insert more than 75 characters.


## 4. Test the password input field character privacy

**Description:** Verify the first text interaction inside the password input field.

**Steps to reproduce:** 
1. Access the Login page
2. Select the password input field
3. Insert more characters

**_Expected results:_** Interacting for the first time with the password field by inputting text, the character privacy is on. The characters should appear as black dots. 


## 5. Test the password input field character privacy setting

**Description:** Verify the functionality of the character privacy setting 

**Steps to reproduce:** 
1. Access the Login page
2. Select the password input field
3. Insert more characters
4. Click on the Show / Hide button 

**_Expected results:_** After inputting some characters inside the password field, a button which hides / unhides the typed characters is displayed and functional on the right side of the password field. 


## 6. Test the login button functionality condition

**Description:** Verify if the functionality condition for the login button works depending on input fields completion and password min limit characters.

**Steps to reproduce:** 
* Case 1:
1. Access the Login page
2. Click on the login button 

* Case 2:
1. Access the Login page
2. Insert an email address / phone number or username în the email input field
3. Click on the login button

* Case 3:
1. Access the Login page
2. Insert a valid / invalid password în the password input field
3. Click on the login button

* Case 4:
1. Access the Login page
2. Insert an email address / phone number or username în the email input field
3. Insert a password containing only 5 or less characters
4. Click on the Login button

**_Expected results:_**  The login button should not work if one of the input text fields is empty or the password contains less than 6 characters. 


## 7. Test the login feature with invalid credentials.

**Description:** Test the login feature by using invalid credentials for email/username/phone number and password.

**Steps to reproduce:** 
* Case 1 (invalid email)
1. Access the Login page
2. Insert an invalid email
3. Insert a random password în it’s input field
4. Click on login button

* Case 2 (invalid username)
1. Access the Login page
2. Insert an invalid username
3. Insert a random password în it’s input field
4. Click on login button

* Case 3 (invalid phone number)
1. Access the Login page
2. Insert an invalid phone number
3. Insert a random password în it’s input field
4. Click on login button

* Case 4 (valid phone number & invalid password)
1. Access the Login page
2. Insert a valid phone number
3. Insert an invalid password 
4. Click on login button

* Case 5 (valid username & invalid password)
1. Access the Login page
2. Insert a valid username
3. Insert an invalid password 
4. Click on login button

* Case 6 (valid email & invalid password)
1. Access the Login page
2. Insert a valid email
3. Insert an invalid password 
4. Click on login button


**_Expected results:_**
After inputting some characters inside the password field, a functional button which hides / unhides the typed characters is displayed on the right side of the password field. 
Attempting to log în using invalid credentials (email / username / phone number / password) will result în an error stating: “Sorry, your password was incorrect. Please double-check your password.”


## 8. Test the login feature with valid credentials.

**Description:** Test the login feature by using valid credentials for email/username/phone number and password.

**Steps to reproduce:** 
* Case 1 (valid email)
1. Access the Login page
2. Insert a valid email
3. Insert a valid password 
4. Click on login button

* Case 2 (valid username)
1. Access the Login page
2. Insert a valid username
3. Insert a valid password 
4. Click on login button

* Case 3 (valid phone number)
1. Access the Login page
2. Insert a valid phone number
3. Insert a valid password 
4. Click on login button

**_Expected results:_** Logging in with valid credentials should redirect the user to the instagram's landing menu.

## 9. Test website compatibility for multiple browsers.
// Non-Functional tests - Compatibility

**Description:** Verify if the website runs properly using different web browsers: Chrome, Safari, Firefox.

**Steps to reproduce:** 
* Case 1 (Chrome)
1. Open Chrome browser
2. Proceed to the Instagram login page 
3. Perform a quick check test

* Case 2 (Firefox)
1. Open Firefox browser
2. Proceed to the Instagram login page 
3. Perform a quick check test

* Case 3 (Safari)
1. Open Safari browser
2. Proceed to the Instagram login page 
3. Perform a quick check test

**_Expected results:_** The website behaves properly having no broken UI assets and all buttons and features are functional. 


## 10. Test the login page behavior under high load conditions.
// Non-Functional tests - Load Test

**Description:** Simulate a large number of authentication requests to the server within a short period of time, to assess how the system handles a heavy load.

**Steps to reproduce:** 
1. Open the testing tool (ex: Apache JMeter)
2. Define a configuration that simulates 500 users attempting to log in simultaneously
3. Run the load test

**_Expected results:_** 
* The response time of the login page should remain within acceptable limits (values can be defined)
* The error rate should be minimal.
* The system's resource utilization, such as CPU, memory, and network usage, are within acceptable limits (values can be defined)
