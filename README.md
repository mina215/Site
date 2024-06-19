# Site
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cars and Bikes</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.php">Home</a></li>
                <li><a href="car-list.php">Cars</a></li>
                <li><a href="bike-list.php">Bikes</a></li>
                <li><a href="parts-list.php">Spare Parts</a></li>
                <li><a href="wash-list.php">Car Wash</a></li>
            </ul>
        </nav>
    </header>

    <section class="slideshow">
        <!-- Slideshow container -->
        <div class="slideshow-container">
            <div class="mySlides fade">
                <img src="slide1.jpg" style="width:100%">
                <div class="text">Slide 1</div>
            </div>
            <div class="mySlides fade">
                <img src="slide2.jpg" style="width:100%">
                <div class="text">Slide 2</div>
            </div>
            <div class="mySlides fade">
                <img src="slide3.jpg" style="width:100%">
                <div class="text">Slide 3</div>
            </div>
        </div>
        <br>
        <div style="text-align:center">
            <span class="dot"></span>
            <span class="dot"></span>
            <span class="dot"></span>
        </div>
    </section>

    <section>
        <h2>Featured Listings</h2>
        <div class="featured-listings">
            <!-- Add PHP code to fetch and display featured listings -->
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Cars and Bikes</p>
    </footer>

    <script src="scripts.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
}

header {
    background-color: #333;
    color: #fff;
    padding: 1em 0;
}

header nav ul {
    list-style: none;
    text-align: center;
}

header nav ul li {
    display: inline;
    margin: 0 15px;
}

header nav ul li a {
    color: #fff;
    text-decoration: none;
}

.slideshow-container {
    max-width: 1000px;
    position: relative;
    margin: auto;
}

.mySlides {
    display: none;
}

.mySlides img {
    width: 100%;
}

.text {
    color: #f2f2f2;
    font-size: 15px;
    padding: 8px 12px;
    position: absolute;
    bottom: 8px;
    width: 100%;
    text-align: center;
}

.dot {
    height: 15px;
    width: 15px;
    margin: 0 2px;
    background-color: #bbb;
    border-radius: 50%;
    display: inline-block;
    transition: background-color 0.6s ease;
}

.active {
    background-color: #717171;
}

.fade {
    -webkit-animation-name: fade;
    -webkit-animation-duration: 1.5s;
    animation-name: fade;
    animation-duration: 1.5s;
}

@-webkit-keyframes fade {
    from {opacity: .4} 
    to {opacity: 1}
}

@keyframes fade {
    from {opacity: .4} 
    to {opacity: 1}
}

footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1em 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}
let slideIndex = 0;
showSlides();

function showSlides() {
    let i;
    let slides = document.getElementsByClassName("mySlides");
    let dots = document.getElementsByClassName("dot");
    for (i = 0; i < slides.length; i++) {
        slides[i].style.display = "none";  
    }
    slideIndex++;
    if (slideIndex > slides.length) {slideIndex = 1}    
    for (i = 0; i < dots.length; i++) {
        dots[i].className = dots[i].className.replace(" active", "");
    }
    slides[slideIndex-1].style.display = "block";  
    dots[slideIndex-1].className += " active";
    setTimeout(showSlides, 2000); // Change image every 2 seconds
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Car Listings</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.php">Home</a></li>
                <li><a href="car-list.php">Cars</a></li>
                <li><a href="bike-list.php">Bikes</a></li>
                <li><a href="parts-list.php">Spare Parts</a></li>
                <li><a href="wash-list.php">Car Wash</a></li>
            </ul>
        </nav>
    </header>

    <section>
        <h2>Car Listings</h2>
        <div class="listings">
            <!-- Add PHP code to fetch and display car listings -->
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Cars and Bikes</p>
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bike Listings</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.php">Home</a></li>
                <li><a href="car-list.php">Cars</a></li>
                <li><a href="bike-list.php">Bikes</a></li>
                <li><a href="parts-list.php">Spare Parts</a></li>
                <li><a href="wash-list.php">Car Wash</a></li>
            </ul>
        </nav>
    </header>

    <section>
        <h2>Bike Listings</h2>
        <div class="listings">
            <!-- Add PHP code to fetch and display bike listings -->
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Cars and Bikes</p>
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Spare Parts Listings</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="index.php">Home</a></li>
                <li><a href="car-list.php">Cars</a></li>
                <li><a href="bike-list.php">Bikes</a></li>
                <li><a href="parts-list.php">Spare Parts</a></li>
                <li><a href="wash-list.php">Car Wash</a></li>
            </ul>
        </nav>
    </header>

    <section>
        <h2>Spare Parts Listings</h2>
        <div class="listings">
            <!-- Add PHP code to fetch and display spare parts listings -->
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Cars and Bikes</p>
    </footer>
</
