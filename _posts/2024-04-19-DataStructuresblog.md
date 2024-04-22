---
toc: true
comments: true
title: MLProject 
layout: post
description: talk about the ml project, what was done, and the irisi testing feature instead of titanic. 
courses: { csp: {week: 30}}
type: plans
---

<style>
/* Style headings */
h1 {
  color: #333;
  font-size: 24px;
  margin-bottom: 10px;
}

h2 {
  color: #555;
  font-size: 20px;
  margin-bottom: 8px;
}

/* Style images */
img {
  max-width: 100%;
  height: auto;
  margin-bottom: 10px;
}

/* Style lists */
ul, ol {
  margin-left: 20px;
  margin-bottom: 10px;
}

/* Style code blocks */
pre {
  background-color: #f4f4f4;
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 10px;
  overflow-x: auto;
}

code {
  font-family: Consolas, Monaco, 'Andale Mono', monospace;
  font-size: 14px;
}

/* Table of Contents (TOC) */
.toc {
  border: 1px solid #ddd;
  border-radius: 4px;
  padding: 10px;
  background-color: #f9f9f9;
}

.toc ul {
  list-style: none;
  padding: 0;
}

.toc li {
  margin-left: 10px;
}

/* Comments */
.comments {
  font-style: italic;
  color: #888;
}

/* Miscellaneous */
body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  margin: 20px;
}
</style>
# Collections
## Blog Python Model code and SQLite Database.
### From VSCode using SQLite3 Editor, show your unique collection/table in the database, and display rows and columns in the table of the SQLite database.
![picture](https://i.ibb.co/30DZwCx/image.png)
### From VSCode model, show your unique code that was created to initialize the table and create test data.
![picture](https://i.ibb.co/C1KK05W/image.png)
![picture](https://i.ibb.co/NZ7nd9C/image.png)
![picture](https://i.ibb.co/VCZmpX9/image.png)
![picture](https://i.ibb.co/Btsb9CT/image.png)
![picture](https://i.ibb.co/8zDKcn5/image.png)

# Lists and Dictionaries
## Blog Python API code and use of List and Dictionaries.
### In VSCode using Debugger, show a list as extracted from the database as Python objects.
### In VSCode use Debugger and list, show two distinct example examples of dictionaries, and show Keys/Values using Debugger.
Here is an example of a list. This code ensures that requests are only allowed from specific origins listed in the predefined list. If a request comes from an allowed origin, the CORS policy is adjusted to allow requests from that origin. So, when I set a breakpoint to this code and run our song picker, the code fails. Once these key values are removed, the code fails to function, and the backend breaks down. 
![picture](https://i.ibb.co/87w9M9M/image.png)
Another instance of a similar situation can be seen in: 
![picture](https://i.ibb.co/m5RD153/image.png)
![picture](https://i.ibb.co/1RKhXXD/image.png)
![picture](https://i.ibb.co/SwkFd7p/image.png)


# APIs and JSON
## Blog Python API code and use of Postman to request and respond with JSON.
### In VSCode, show Python API code definition for request and response using GET, POST, UPDATE methods. Discuss algorithmic conditions used to direct request to appropriate Python method based on request method.
This can be seen in the register function. This piece of code manages user registration, so when someone tries to register, it checks if they provided a username, password, and confirmation. If any of these are missing, it tells them to fill them in. If everything is provided, it checks if the username is already taken. If not, it adds the new user to the system. If the username is already taken, it tells the user to pick a different one.
![picture](https://i.ibb.co/ZfXvbsp/image.png)
![picture](https://i.ibb.co/x3k82MF/image.png)
Another Instance:
![picture]https://i.ibb.co/Dzt3jwS/image.png)
### In VSCode, show algorithmic conditions used to validate data on a POST condition.
![picture](https://i.ibb.co/MhQ5ZK7/image.png)
### In Postman, show URL request and Body requirements for GET, POST, and UPDATE methods.
![picture](https://i.ibb.co/1GR5GYk/image.png) 
### In Postman, show the JSON response data for 200 success conditions on GET, POST, and UPDATE methods.
![picture](https://i.ibb.co/9yssGqP/image.png)
### In Postman, show the JSON response for error for 400 when missing body on a POST request.
![picture](https://i.ibb.co/ZBLfcLP/image.png) 
### In Postman, show the JSON response for error for 404 when providing an unknown user ID to a UPDATE request.
![picture](https://i.ibb.co/ZKxTPkm/image.png)
# Frontend
## Blog JavaScript API fetch code and formatting code to display JSON.
### In Chrome inspect, show response of JSON objects from fetch of GET, POST, and UPDATE methods.
Code breaking in login
![picture](https://i.ibb.co/9V3qn9Z/image.png)
This is where i decided to set the breakpoint, on the fetch code in the frontend. 
![picture](https://i.ibb.co/PtBb4pt/image.png)
### In the Chrome browser, show a demo (GET) of obtaining an Array of JSON objects that are formatted into the browsers screen.
![picture](https://i.ibb.co/PtBb4pt/image.png)
### In JavaScript code, describe fetch and method that obtained the Array of JSON objects.
“fetch(url, authOptions)” gets the url from the backend server (http://127.0.0.1:8088) followed by the suffix “/api/users/authenticate”. This is first done to authenticate the user, before they gain access to the array of JSON objects that are formatted into the browser’s screen. When the login is successful, the page is redirected to the Database of users that was formatted in the browser. Next, the url is passed as “http://127.0.0.1:8088/api/users/” since we want to obtain the actual JSON data of the users in the database. Another fetch is done with the url and when the data is fetched, HTML formats all of it into a table, to make it resemble the SQLite database.

#### In JavaScript code, show code that performs iteration and formatting of data into HTML.
![picture](https://i.ibb.co/ZfMQP24/image.png)
### In the Chrome browser, show a demo (POST or UPDATE) gathering and sending input and receiving a response that show update. Repeat this demo showing both success and failure.
![picture](https://i.ibb.co/S3rjKXR/image.png)
![picture](https://i.ibb.co/r7DhqZx/image.png)
![picture](https://i.ibb.co/xDHHvKk/image.png)
![picture](https://i.ibb.co/S6F2jyS/image.png)
#### In JavaScript code, show and describe code that handles success. Describe how code shows success to the user in the Chrome Browser screen.
![picture](https://i.ibb.co/w0vhy8w/image.png)
This code simply redirects you to the database as a result of you logging in.
#### In JavaScript code, show and describe code that handles failure. Describe how the code shows failure to the user in the Chrome Browser screen.
![picture](https://i.ibb.co/HGfbz2T/image.png)
This code simply redirects you to an error for not being able to login properly. 
