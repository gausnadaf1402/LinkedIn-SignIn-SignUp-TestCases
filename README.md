This repository provides guidelines for performing manual testing on the LinkedIn Sign-In and Sign-Up functionalities. The goal is to ensure the correct behavior of the authentication system, focusing on both positive and negative test scenarios.

** Table of Contents
. Introduction
. Prerequisites
. Test Cases
  . Sign-Up Tests
  . Sign-In Tests
  . Password Reset Tests
. Test Execution Process
. Expected Results

This document outlines the manual testing procedures for the Sign-Up and Sign-In pages of LinkedIn. It is designed to verify that new users can create accounts, existing users can log in, and appropriate error messages are shown for invalid input.

** Prerequisites:-
Before starting the testing process, ensure the following:

We have access to a stable internet connection.
We  can access LinkedIn’s web application via a browser.
We have multiple valid and invalid email addresses to test various scenarios.

** Test Cases:- 
Sign-Up Tests
Test Case ID	Test Case Description	Steps	Actual Result Expected Result Status
TC01	Sign-Up with valid details	1. Navigate to LinkedIn sign-up page. 2. Enter valid details (name, email, password). 3. Submit the form.	User is successfully registered, and a confirmation email is sent.
TC02	Sign-Up with an invalid email	1. Navigate to sign-up page. 2. Enter an invalid email (e.g., user@domain). 3. Submit the form.	Error message prompts user to enter a valid email.
TC03	Sign-Up with already registered email	1. Enter an email that is already registered. 2. Fill in the rest of the form. 3. Submit the form.	Error message indicating the email is already in use.

Sign-In Tests
Test Case ID	Test Case Description	Steps	Expected Result
TC04	Sign-In with valid credentials	1. Navigate to LinkedIn sign-in page. 2. Enter valid email and password. 3. Click "Sign In."	User is successfully logged in and redirected to the homepage.
TC05	Sign-In with invalid password	1. Navigate to sign-in page. 2. Enter a valid email and incorrect password. 3. Submit the form.	Error message prompts user that the password is incorrect.
TC06	Sign-In with unregistered email	1. Enter an email that is not registered. 2. Submit the form.	Error message indicating the email is not found. Password Reset Tests Test Case ID	Test Case Description	Steps	Expected Result
TC07	Reset password with valid email	1. Navigate to "Forgot Password" page. 2. Enter a valid registered email. 3. Follow the instructions sent via email.	User receives a reset email and can successfully reset the password.
TC08	Reset password with unregistered email	1. Enter an unregistered email on "Forgot Password" page. 2. Submit the form.	Error message indicating the email is not associated with an account.

** Test Execution Process: 
Prepare the Test Environment:
Open a web browser (e.g., Chrome, Firefox).
Clear cache and cookies to avoid session-related issues.
Execute Test Cases:

Follow the steps listed in each test case.
Use different combinations of inputs (valid and invalid) to test the boundary conditions.
Record the results for each test case, including the actual outcome.
