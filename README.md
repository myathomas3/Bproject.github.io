<html lang="en">
<head>
   <header>
    <a class="donate-button" href="https://your-donation-link.com">Donate</a>
</header>
   <img src="Boxproject logo.png" alt="logo" style="width: 150px; height: auto;">
   
   <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Carousel with Automatic Transitions</title>
    <link rel="stylesheet" href="styles">

    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Website Title</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            background-color: #3498db; /* Blue background color */
            color: #000; /* Black text color */
            font-family: Arial, sans-serif;
        }
    </style>
</head>

<body>

   <img id="logo" src="Boxproject logo.png" alt="Logo" width="100" height="100">
   <script>
    // Get a reference to the logo element
    const logo = document.getElementById('logo');

    // Add a click event listener to the logo
    logo.addEventListener('click', function() {
        // Redirect to the home page URL
        window.location.href = 'https://myathomas3.github.io/Bproject.github.io/'; // Replace 'home.html' with your actual home page URL
    });
</script>
   
   <div class="carousel-container">
        <div class="carousel-slide">
            <img src="(1).png" alt="Image 1">
            <div class="caption">Caption for Image 2</div>
        </div>
        <div class="carousel-slide">
            <img src="(2).png" alt="Image 2">
            <div class="caption">Caption for Image 2</div>
        </div>
        <div class="carousel-slide">
            <img src="(3).png" alt="Image 3">
            <div class="caption">Caption for Image 2</div>
        </div>
         <div class="carousel-slide">
            <img src="(4).png" alt="Image 4">
             <div class="caption">Caption for Image 2</div>
        </div>
         <div class="carousel-slide">
            <img src="(5).png" alt="Image 5">
             <div class="caption">Caption for Image 2</div>
        </div>
         <div class="carousel-slide">
            <img src="(6).png" alt="Image 6">
             <div class="caption">Caption for Image 2</div>
        </div>
         <div class="carousel-slide">
            <img src="(7).png" alt="Image 7">
             <div class="caption">Caption for Image 2</div>
        </div>
         <div class="carousel-slide">
            <img src="(8).png" alt="Image 8">
             <div class="caption">Caption for Image 2</div>
        </div>
         <div class="carousel-slide">
            <img src="(9).png" alt="Image 9">
             <div class="caption">Caption for Image 2</div>
        </div>
         <div class="carousel-slide">
            <img src="(10).png" alt="Image 10">
             <div class="caption">Caption for Image 2</div>
        </div>
         <div class="carousel-slide">
            <img src="(11).png" alt="Image 11">
             <div class="caption">Caption for Image 2</div>
        </div>
         <div class="carousel-slide">
            <img src="(12).png" alt="Image 12">
            <div class="caption">Caption for Image 2</div>
        </div>
      
    </div>
    <button id="prev">Previous</button>
    <button id="next">Next</button>

    <script>
        const prevButton = document.getElementById('prev');
        const nextButton = document.getElementById('next');
        const slides = document.querySelectorAll('.carousel-slide');
        let currentSlide = 0;

        function showSlide(index) {
            slides.forEach((slide, i) => {
                slide.style.display = i === index ? 'block' : 'none';
            });
        }

        prevButton.addEventListener('click', () => {
            currentSlide = (currentSlide - 1 + slides.length) % slides.length;
            showSlide(currentSlide);
        });

        nextButton.addEventListener('click', () => {
            currentSlide = (currentSlide + 1) % slides.length;
            showSlide(currentSlide);
        });

        function autoAdvance() {
            currentSlide = (currentSlide + 1) % slides.length;
            showSlide(currentSlide);
        }

        // Set an interval for automatic transitions (e.g., every 5 seconds)
        const interval = setInterval(autoAdvance, 3000);

        // Stop the interval when the user clicks on the "Previous" or "Next" buttons
        prevButton.addEventListener('click', () => {
            clearInterval(interval);
        });

        nextButton.addEventListener('click', () => {
            clearInterval(interval);
        });

        // Initial display
        showSlide(currentSlide);
    </script>
    <header>
        <h1>The Box Project</h1>
        <nav>
            <ul>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
               <li><a href="#">Contact</a></li> 
      <p>
        The Box Project is a program of the Community Foundation of Northwest Mississippi, an accredited foundation with the Council on Foundations’ National Standards for U.S. Community Foundations. It is governed by the Community Foundation’s Board of Directors. We encourage you to investigate before you donate. Click here to read more about the Community Foundation and its finances. Click here for more information about the Box Project and its relationship to the Community Foundation of Northwest Mississippi.
      </p>
    </div>
  );
};

            </ul>
        </nav>
    </header>
    <main>
        <section>
            <h2>Mission</h2>
            <p>The Box Project offers a unique opportunity to give back. We are distinct because we create supportive, personal relationships directly between a sponsor family and a family in need living in rural America. The Box Project acts as matchmaker, pairing our “sponsor” volunteers with carefully screened individuals or families that need help. The sponsors offer long term, meaningful interactions including encouragement, advice, and boxes of needed supplies about once a month.</p>
        </section>
        <section>
            <h2>Services</h2>
            <ul>
                <li>Service 1</li>
                <li>Service 2</li>
                <li>Service 3</li>
            </ul>
        </section>
    </main>
    <section>
        <h2>Connect with Us</h2>
        <div id="badges">
  <a href="https://www.facebook.com/TBP1962/">
    <img src="https://img.shields.io/badge/facebook-blue?style=for-the-badge&logo=facebook&logoColor=white" alt="facebook Badge"/>
  </a>
  <a href="https://www.youtube.com/channel/UCu-tEnjTcYvVlTRcvvCJw3g">
    <img src="https://img.shields.io/badge/YouTube-red?style=for-the-badge&logo=youtube&logoColor=white" alt="Youtube Badge"/>
  </a>
  <a href="http://www.twitter.com/@TBP1962">
    <img src="https://img.shields.io/badge/Twitter-blue?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter Badge"/>
  </a>
</div>
        
    </section>
    <footer>
        <p>&copy; 2023 Your Website. All rights reserved.</p>
    </footer>
</body>
</html>
