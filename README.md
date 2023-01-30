# extending_testing_challenge_one

## States
* Home page
* Sign up page
* Login page
* User home page

## Events
* Navigating to home page
* Navigating to login page
* Navigating to sign up page
* Logging in
* Signing up
* Logging out

## Causality
* __Navigating to home page__ takes user from __sign up page__ or __login page__ to __home page__
* __Navigating to login page__ takes user from __home page__ or __sign up page__ to __login page__
* __Navigating to sign up page__ takes user from __home page__ or __login page__ to __sign up page__
* __Signing in__ takes user from __sign up page__ to __login page__
* __Logging in__ takes user from __login page__ to __user page__
* __Logging out__ takes user from __user home page__ to __home page__

## State transition diagram
![challenge 1](https://user-images.githubusercontent.com/115627873/215474633-41bde454-a3e5-419c-9e05-d2654b613bd5.png)

## State transition table
| Initial State | Event | Next State |
|-|-|-|
|Home page|Navigating to sign up page|Sign up page|
|Home page|Navigating to login page|Login page|
|Sign up page|Navigating to home page|Home page|
|Sign up page|Navigating to login page|Login page|
|Sign up page|Signing up|Login page|
|Login page|Navigating to home page|Home page|
|Login page|Navigating to sign up page|Sign up page|
|Login page|Logging in|User home page|
|User home page|Logging out|Home page|

## Test case
1. Start => Home page
2. Home page => Sign up page (navigating)
3.  Sign up page => Home page (navigating)
4.  Home page => Login page (navigating)
5.  Login page => Sign up page (navigating)
6.  Sign up page => Login page (navigating)
7.  Login page => Home page (navigating)
8.  Home page => Sign up page (navigating)
9. Sign up page => Login page (sign up)
10. Login page => User home page (login)
11. User home page => Home page (logout)
