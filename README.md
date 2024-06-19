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
