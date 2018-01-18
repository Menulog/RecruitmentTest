Menulog Engineer Recruitment Test
==================================

Thank you for taking the time to do our technical test. It consists of two parts:

* [A coding test](#coding-test)
* [A few technical questions](#technical-questions)

In order to avoid bounced emails we would like you to submit your results by uploading the relevant zip file to a shared Google Drive folder. In order to obtain the URL for this folder please supply your Gmail or Google-based email address to either your agent or the Menulog member of staff who assigned you the test.

Please make this a **single** zip file named **{yourname}-{role-applied-for}.zip** containing:

1. A single markdown file with the answers to the technical questions
2. One folder containing the technical test

## Coding Test

Menulog, part of the Just Eat group, has a public API available at [https://public.je-apis.com/](https://public.je-apis.com/) that you can use to get restaurant information, including restaurant details and delivery information.

### How to use the API

The API requires you to specify a set of valid request headers.
```
Accept-Tenant: uk
Accept-Language: en-GB
Accept-Charset: utf-8
Authorization: Basic VGVjaFRlc3RBUEk6dXNlcjI=
Host: public.je-apis.com
```
Some examples:
* [https://public.je-apis.com/restaurants?q=se19](https://public.je-apis.com/restaurants?q=se19) returns a list of restaurants that deliver to an outcode, including some basic restaurant information (for outcode = se19)

* [https://public.je-apis.com/restaurants/17266/menus](http://public.je-apis.com/restaurants/17266/menus) returns a list of menues for a restaurant (for restaurantid = 17266)

* [https://public.je-apis.com/menus/57443/productcategories](https://public.je-apis.com/menus/57443/productcategories) returns a list of categories for a menu (for menuid = 57433)

* [https://public.je-apis.com/menus/57443/productcategories/5/products](https://public.je-apis.com/menus/57443/productcategories/5/products) returns a list of products for a given category for a given menu (for. menuid = 57433 & categoryid = 5)

### What you need to do

The task is to create an application that allows users to enter an outcode (postcode) as a parameter and get back a list of restaurants that deliver to that outcode, including the following information:

* Name
* Average rating
* Restaurant logo
* A link to the restaurant on the JUST EAT website
* A list of products the restaurant sell

The restaurants should be ordered from highest average rating to lowest average rating and the restaurants should be loaded using some form of async connection.

Please take the time to write code and any tests to the standard you would expect in a real application.

### Platform Choice

You can create the application as either a command line application, web application or mobile application in any of the following platforms

* .NET (VS 2015), PHP (v5.6+) or JavaScript for command line applications
* .NET (VS 2015), PHP (v5.6+) or JavaScript for web applications
* iOS, Android or Windows Mobile for mobile applications

Think about the type of work you would like to do at Menulog and **choose an appropriate application type and platform** to showcase your skills and expertise.

### Task requirements

Feel free to spend as much or as little time on the exercise as you like as long as the following requirements have been met.  

* Please complete the user story below.
* Your code should compile and run in one step.
* Feel free to use whatever frameworks / libraries / packages you like.

### User Story

As a **user running the application**  
I can **view a list of restaurants in a user submitted outcode (ex. SE19)**  
So that **I know which restaurants are currently available**

If you have chosen a native mobile application platform please also include the following:

As a **user running the application**  
I can **view the the restaurant logo along side restaurant information**  
So that **I know exactly which restaurants are currently available**

As a **user running the application**  
I can **use GPS to find my current postcode to retrieve restaurant results**  
So that **I don't need to type it in**

#### Acceptance criteria

- For the known outcode se19, results are returned
- The Name, Cuisine Types and Rating of the restaurant are displayed

### Functional Testing [OPTIONAL]

Write a functional test (both Gherkin scenario and code implementation) which

* Returns a list of restaurants, if the given the postcode is valid; and
* Displays an error message on the site, if the postcode is invalid.

Describe how to run the tests.

# Technical Questions

Please answer the following questions in a markdown file called `Answers to technical questions.md`.

1. How long did you spend on the coding test? What would you add to your solution if you had more time? If you didn't spend much time on the coding test then use this as an opportunity to explain what you would add.
2. What was the most useful feature that was added to the latest version of your chosen language? Please include a snippet of code that shows how you've used it.
3. How would you automate the testing of the solution you built?
4. What's your favourite library? Why?
5. How would you improve the customer experience on [Menulog](https://www.menulog.com.au)?
6. How would you improve the JUST EAT APIs that you just used?
7. How would you track down a performance issue in production? Have you ever had to do this?
8. Please describe yourself using JSON.

#### Thanks for your time, we look forward to hearing from you! The [Menulog and Just Eat Tech team](http://github.com/justeat)
