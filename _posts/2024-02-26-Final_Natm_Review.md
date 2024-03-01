---
toc: true
comments: true
title: natm review
layout: post
description: CPT Final Review
courses: { csp: {week: 18}}
type: plans
---

# Project Summary: 
- Our CPT project allows players to access a game universe, where they can build their own games, test it, draw new things, and play some cool games. They can personalize their accounts by choosing their favorite game, and they can update their username and password whenever they want. 

# My Features:
- My main additions and features to the project was the front end. I worked on a lot of the front end homepage, as well as the game list page, and almost every game you see in the games list. I built in a working filter to the game page. On top of that I've added a change color feature on the homepage, along with snowflake features. This add some customizability the homepage. Another thing I've done was add a drop-down section with frequently asked questions, as well as featured games area.    

### Collegeboard Requirments A and B
**[CollegeBoard requirements documents A and B](https://apcentral.collegeboard.org/media/pdf/ap-csp-student-task-directions.pdf)**

<br>

# CollegeBoard Requirements:

## Component A
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CollegeBoard requirements summary: Component A</title>
    <style>
       table {
    width: 120%;
    border-collapse: collapse;
    margin-top: 20px;
    }
    </style>
</head>
<body>
    <table>
        <thead>
            <tr>
                <th>CB Requirement</th>
                <th>Fulfillment</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Instructions for input from one of the following: the user, a device, an online datas stream, a file</td>
                <td>Our project includes a login feature as well as asign up fetaure that the user can log in and sign up through. They will be prompted to enter credentials in order to create the account, and will be asked for thos exact credentials later in order to sign in to their account. They can update those features after logging in, and even add a favorite game. it inputs their name, username, password, and favorite game and email.  

                The layout of the website is really easy to follow, making it easy for users to figure where they need to go and what they need to do. However, if it isnt clear enough, the site homepage directs users to the login and game list websites, as well the featured games and slideshow on the homepage. 
                <img src="/updatepagepage" alt="Login page">
                <img src="_posts/homepagedesc.png" alt="Sign up page">
                </td>
            </tr>
            <tr>
                <td>Use of at least one list (or other collection type) to represent a collection of data that is stored and used to manage program complexity and help fulfill the users purpose</td>
                <td>For storing users data, we used an escalate database that stores the user information, including their ‘favorite’, ‘username’, and ‘password’.  
                <img src="_posts/sqlitedb.png" alt="Database">
                </td>
            </tr>
            <tr>
                <td>At least one procedure that contributed to the program’s intended purpose where you have defined: the name, return type, one or more parameters</td>
                <td> The following procedure checks for the validity of the login information (obtained from the backend using a `fetch` function) and allows the user to login and access their college application tracker. It also redirects users to the specific error pages based on different error cases.
                <img src="retunrtype" alt="Fetch function">
                <img src="_posts/404return.png" alt="Fetch">
                </td>
            </tr>
            <tr>
                <td>An algorithm that includes sequencing, selection, and iteration that is in the body of the selected procedure
                </td>
                <td> This piece of code is from our user.py API file. Of course I'm in checking feature our database will iterate through the different uid's obtained from the request payload and it will change and update the information of the user as user requests it.
                <img src="_posts/requestpayload.png" alt="404requests">
                </td>
            </tr>
            <tr>
                <td>Calls to your student-developed procedure</td>
                <td> This code uses the get request in order to read and extract all the information, as in the users and their information, that is from our database. This will be displayed in our front end.
                <img src="_posts/getrequests.png" alt="GET">
                </td>
            </tr>
            <tr>
                <td>Instructions for output (tactile, audible, visual, or) based on input and program functionality</td>
                <td> Basic FAQ content to lead the user to usew site/pretty selfexplanatory otherwise
                <img src="_posts/faqlikecontent.png" alt="Output">
                </td>
            </tr>
        </tbody>
    </table>
</body>
</html>

<br>

## Component B
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CollegeBoard requirements summary: Component B</title>
    <style>
       table {
    width: 120%;
    border-collapse: collapse;
    margin-top: 20px;
    }
    </style>
</head>
<body>
    <table>
        <thead>
            <tr>
                <th>CB Requirement</th>
                <th>Fulfillment</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Input to your program</td>
                <td> The video showcases user pressing buttons, and playing games and inputting into the prgoram</td>
            </tr>
            <tr>
                <td>At least one aspect of the functionality of your program</td>
                <td> The program responds and does the correct move for the player.</td>
            </tr>
            <tr>
                <td>Output produced by your program</td>
                <td> The output done by this would be the succesful move placement for the player playing the game, or maybe the filter working just as it should.</td>
            </tr>
            <tr>
                <td>DOES NOT contain any distinguishing information about yourself</td>
                <td> This video does not contain and distinguishing information about myself.</td>
            </tr>
            <tr>
                <td>DOES NOT contain voice narration (though text captions are encouraged</td>
                <td> uses captions over voice naration</td>
            </tr>
            <tr>
                <td>Video is either .webm, .mp4, .wmv, .avi, or .mov format</td>
                <td> The video is in the .mp4 format.</td>
            </tr>
            <tr>
                <td>Video is no more than 1 minute in length</td>
                <td> The video is less than 1 minute.</td>
            </tr>
            <tr>
                <td>Video is no more than 30MB file size</td>
                <td> The file size is less than 30 MB.</td>
            </tr>
        </tbody>
    </table>
</body>
</html>

**[Video link](https://drive.google.com/file/d/16MtThKfqq40PQfb5RhVIhWJ7yoI_u9TF/view?usp=sharing)**

<br>

# The Key Commits:
[Homepage Major Commit, Animation + Styles + Bubbling added](https://github.com/ShakeSphereStuff/GUIFor2DGameEngine/commit/78db562c9f8baf46934faf52d1458a2e26d5cc16)<br><br>
[Gamelist commit, filter system plus bubbles](https://github.com/ShakeSphereStuff/GUIFor2DGameEngine/commit/293b49081a8978a255ecdd6c28a7ad569ac83123)<br><br>
[tictactoe game commit](https://github.com/ShakeSphereStuff/GUIFor2DGameEngine/commit/cb50af3c5e5b163b63aa7bfadbe6d00cadcfb785)<br><br>
[Ping Pong Game Commit](https://github.com/ShakeSphereStuff/GUIFor2DGameEngine/commit/a3ddb7b56a279e02f333030cad40aa766d2265db)