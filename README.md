# styles.css
html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Page</title>
    <link rel="stylesheet" href="style.css"> <!-- Link external CSS -->
</head>
<body>

    <!-- Navigation Bar -->
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>

    <!-- Content Section -->
    <div class="container">
        <div class="box">Box 1</div>
        <div class="box">Box 2</div>
        <div class="box">Box 3</div>
    </div>

</body>
</html>

/* General Styling */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

/* Navigation Bar */
nav {
    background-color: #007BFF;
    padding: 10px 0;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 18px;
}

/* Flexbox Layout */
.container {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap; /* Ensures items wrap on smaller screens */
    padding: 20px;
}

.box {
    background-color: white;
    padding: 20px;
    margin: 10px;
    width: 30%; /* Each box takes 30% width */
    text-align: center;
    border: 2px solid #007BFF;
    border-radius: 10px;
    box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.2);
}

/* Media Queries for Responsive Design */
@media (max-width: 768px) {
    .container {
        flex-direction: column; /* Stack boxes vertically */
        align-items: center;
    }

    .box {
        width: 80%; /* Full width on smaller screens */
 @media (max-width: 480px) {
    nav ul {
        flex-direction: column; /* Stack menu items vertically */
    }

    nav ul li {
        margin: 10px 0;
