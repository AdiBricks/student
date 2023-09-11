---
#toc: true
comments: true
title: Hacks Learned Week 3
layout: post
description: Hacks Learned Week 3
courses: { csp: {week: 3}}
type: hacks
---





Different Types of hacks and what they mean:
Event Listener Setup:

searchButton.addEventListener('click', function () { ... });
Sets up a click event listener on the search button to trigger the search when clicked.
Fetching Data from YouTube API:

fetch(https://www.googleapis.com/youtube/v3/search?key=${apiKey}&part=snippet&q=${query}`)`
Initiates a request to the YouTube Data API to search for videos based on the user's query.
Displaying Search Results:

searchResults.innerHTML = '';
Clears any previous search results from the webpage.
searchResults.appendChild(resultItem);
Appends each video search result to the webpage.
Extracting Video Data:

Extracts video details like title, description, thumbnail, and video ID from the API response.
Error Handling:

.catch(error => { ... });
Handles errors, logging them to the console if something goes wrong during the fetch or data processing.
These parts are crucial for understanding how the code works and its core functionality.

Clearing the Board (clear_screen):
Function definition to clear the screen, making it appear as if the board is refreshed:

def clear_screen():
    if os.name == 'nt':
        os.system('cls')
    else:
        os.system('clear')

To make the Computer move:
def make_ai_move(board):
    while True:
        col = random.randint(0, len(board[0]) - 1)
        if is_valid_move(board, col):
            return col
