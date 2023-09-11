---
title: Youtube Search
layout: post
description: Youtube search
courses: {'csp': {'week': 3}}
categories: ['C4.0']
type: hacks
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>YouTube Search</title>
</head>
<body>
    <h1>YouTube Search</h1>
    <input type="text" id="searchQuery" placeholder="Enter your search query">
    <button id="searchButton">Search</button>
    <div id="searchResults"></div>

    <script>
        const searchQueryInput = document.getElementById('searchQuery');
        const searchButton = document.getElementById('searchButton');
        const searchResults = document.getElementById('searchResults');

        // Replace 'YOUR_API_KEY' with your actual YouTube Data API key.
        const apiKey = 'AIzaSyBY7-YaZ8a4H0U4YClle0koQhxuJbBvaJY';

        searchButton.addEventListener('click', function () {
            const query = searchQueryInput.value.trim();
            if (query) {
                // Perform a search using the YouTube Data API.
                fetch(`https://www.googleapis.com/youtube/v3/search?key=${apiKey}&part=snippet&q=${query}`)
                    .then(response => response.json())
                    .then(data => {
                        searchResults.innerHTML = '';

                        // Display search results.
                        data.items.forEach(item => {
                            const videoId = item.id.videoId;
                            const title = item.snippet.title;
                            const description = item.snippet.description;
                            const thumbnail = item.snippet.thumbnails.default.url;

                            const resultItem = document.createElement('div');
                            resultItem.innerHTML = `
                                <h3>${title}</h3>
                                <p>${description}</p>
                                <a href="https://www.youtube.com/watch?v=${videoId}" target="_blank">
                                    <img src="${thumbnail}" alt="${title}">
                                </a>
                            `;
                            searchResults.appendChild(resultItem);
                        });
                    })
                    .catch(error => {
                        console.error('Error fetching data:', error);
                    });
            }
        });
    </script>
</body>
</html>

