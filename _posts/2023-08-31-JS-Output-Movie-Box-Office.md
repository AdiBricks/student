---
title: Box Office Numbers.
toc: true
layout: post
description: JS Output for Movie Box Office Numbers! 
courses: { csp: {week: 2}}
type: hacks
---


%%html

<!-- Head contains information to Support the Document -->
<head>
    <!-- load jQuery and DataTables output style and scripts -->
    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.13.4/css/jquery.dataTables.min.css">
    <script type="text/javascript" language="javascript" src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <script>var define = null;</script>
    <script type="text/javascript" language="javascript" src="https://cdn.datatables.net/1.13.4/js/jquery.dataTables.min.js"></script>
</head>

<!-- Body contains the contents of the Document -->
<body>
    <table id="demo" class="table">
        <thead>
            <tr>
                <th>Ranking</th>
                <th>Movie Title</th>
                <th>Year</th>
                <th>Gross</th>
                <th>Company</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1</td>
                <td>Avatar</td>
                <td>2009</td>
                <td>$2,923,706,026</td>
                <td>Disney</td>
            </tr>
            <tr>
                <td>2</td>
                <td>Avengers Endgame</td>
                <td>2019</td>
                <td>$2,799,439,100</td>
                <td>Disney</td>
            </tr>
            <tr>
                <td>3</td>
                <td>Avatar The Way Of Water</td>
                <td>2022</td>
                <td>$2,320,250,281</td>
                <td>Disney</td>
            </tr>
            <tr>
                <td>4</td>
                <td>Titanic</td>
                <td>1997</td>
                <td>$2,264,743,305</td>
                <td>Disney</td>
            </tr>
            <tr>
                <td>5</td>
                <td>Star Wars: Episode VII - The Force Awakens</td>
                <td>2015</td>
                <td>$2,071,310,218</td>
                <td>Disney</td>
            </tr>
            <tr>
                <td>6</td>
                <td>Avengers: Infinity War</td>
                <td>2018</td>
                <td>$2,052,415,039</td>
                <td>Disney</td>
            </tr>
            <tr>
                <td>7</td>
                <td>Spider-Man: No Way Home</td>
                <td>2021</td>
                <td>$1,921,847,111</td>
                <td>Sony Pictures</td>
            </tr>
            <tr>
                <td>8</td>
                <td>Jurrasic World</td>
                <td>2015</td>
                <td>$1,671,537,444</td>
                <td>Universal Pictures</td>
            </tr>
            <tr>
                <td>9</td>
                <td>Lion King</td>
                <td>2019</td>
                <td>$1,663,075,40</td>
                <td>Disney</td>
            </tr>
            <tr>
                <td>10</td>
                <td>The Avengers</td>
                <td>2012</td>
                <td>$1,520,538,536</td>
                <td>Disney</td>
            </tr>
        </tbody>
    </table>
</body>

<!-- Script is used to embed executable code -->
<script>
    $("#demo").DataTable();
</script>