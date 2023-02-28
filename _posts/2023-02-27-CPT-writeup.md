---
toc: true
layout: post
description: CPT Submissions (Trimester 2)
categories: [Trimester 2]
title: Tri 2 CPT Write-Up
---

# Video

My video demonstration of my feature can be found [here](https://www.youtube.com/watch?v=g4fpVEaYKEI). 

# Write-Up (Location Tracker System)

## 3a.  

### 3.a.i.

This program is meant to provide a quick and simple method to track the current location of others, in context customers and businesses through their phone numbers.

### 3.a.ii.

This program allows a user to not only input their phone number, but the user can also input their own User ID, creating their own unique entires in the API. The user does this by first defining under what name the inputted phone number goes under. These entries are all persistent as well, so even if the page is closed and reopened, the entries remain. 


### 3.a.iii.

The inputs of the program are the user's typed entries into the form for which User ID and Phone Number are taken. The program collects this data and runs an algorithm in the backend to determine the phone number's location and timezone - depending on if the user's entries met the requirements such as filling out all fields - and then update an existing API and completely formats the attributes in a table. 

## 3b.

### 3.b.i.

![Screenshot 2023-02-27 195428](https://user-images.githubusercontent.com/51098969/221749496-f20b4ea9-0f88-42cf-a0d0-1fa4cec8d9f5.jpg)

### 3.b.ii.

![Screenshot 2023-02-27 195329](https://user-images.githubusercontent.com/51098969/221749402-dbf8c084-6894-4dfa-aadb-9829dc2a17b1.jpg)

### 3.b.iii.

The name of the variable representing the collection type is "data".

### 3.b.iv.

The data that my list contains is extremely vital to my program since it contains multiple unique attributes about the user's phone number for the entry. This is absolutely vital to the program as it is able to fetch, create, and store the recieved data in order to populate the tables for when the user decides to view the logged phone numbers of a specific User ID. 

### 3.b.v.

Without the variable "data", everything will become inefficient as the program would then require some sort of individual variable for each and every unique attribute. This would unneedingly lengthen my code and make it much too bulky and complex. 


## 3.c.

### 3.c.i.

![Screenshot 2023-02-27 200312](https://user-images.githubusercontent.com/51098969/221750730-6854376d-d8ef-49fe-ad3e-7d8f16f3bd35.jpg)

### 3.c.ii.

![Screenshot 2023-02-27 200535](https://user-images.githubusercontent.com/51098969/221750978-9e56b26f-89bc-4089-ab89-a1226d02a606.jpg)

### 3.c.iii.

The procedure here is `getPhoneData`. First, the function makes a fetch request to the backend, where an app route to an specified API was defined, passing in the retrieved user value as a query parameter. The function then clears the current displayed table. When the response is received, it is parsed as JSON, and if the resulting array has length greater than zero, the function populates the current table with a new set of rows, one for each row that was received. This procedure is called twice when data needs to be fetched, once when the data needs to be initially populated when the site is visited and again when the 'submit' button is pressed, which sends a form to the backend and calls a function to load new data associated with that user.

### 3.c.iv.

![Screenshot 2023-02-27 201847](https://user-images.githubusercontent.com/51098969/221752597-57318f3a-15d5-4639-8ee1-a22b9f1a3c50.jpg)

My code has the ability to collect input data from a web form using document.getElementById, and proceed to use selection to check if the User ID / Phone Number field is empty or invalid, and if it is, it displays an alert to the user and returns from the function. If the username field is not empty, the function constructs a data object using sequencing, which contains the input values collected earlier. The function then constructs a requestOptions object also using sequencing which includes the data object, and specifies the HTTP method and content type headers for a POST request. The function then uses iteration, in the form of a try-catch block, to handle errors that may occur during the fetch request. Finally, the function uses fetch to send a POST request to a specified URL and logs the success response to the console, as well as displaying an alert to the user.


## 3.d

### 3.d.i.

#### Call One
The user inputs both the attributes on the form, being the User ID and a valid Phone Number and clicks on the "Submit" button. The first call to procedure passes a non-empty User ID and all other required arguments to add a new entry to the system. This call will send this data to the backend, execute the entire algorithm, constructing the data object, constructing the and sending a POST request to the specified API with the data object as the request body. If the request is successful, a success message will be logged to the console and an alert will be shown to the user indicating that the inventory has been added.


#### Call Two
The user inputs both the attributes on the form, being the User ID and a Phone Number, however this Phone Number is invalid and does not exist. This call will execute only the selection code segment that checks if the phone number is valid. Since the passed argument is an invalid Phone Number, an alert will be shown to the user indicating that the entered number is invalid. The rest of the code segments will not execute, and no request will be sent to the server.



### 3.d.ii.

#### Condition(s) tested by Call One
The given code includes two conditional statements to test certain conditions. The first conditional statement tests whether the username variable is empty, which is checked using the if statement if (user === ""). The second conditional statement includes an if statement "if (!phoneNumberRegex.test(phoneNumberInput.value)) {" to test the validity of the phone number inputted.


#### Condition(s) tested by Call Two
The second conditional statement is not explicitly shown in the code block, but is present in the .catch() block of the fetch() method call. This is a catch-all statement that executes if there are any errors during the HTTP request or response, such as a network error or a server-side error. 


### 3.d.iii.

#### Results of Call One
If the username is indeed filled and a valid phone number is entered, then an alert is displayed with the message "Data has been entered successfully." and the procedure continues and delivers using the return statement.


#### Results of Call Two
If such an error occurs, then the catch block logs the error to the console using console.error(error). An alert is displayed with the message "Invalid phone number format".
