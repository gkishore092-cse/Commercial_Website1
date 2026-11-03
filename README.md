# Ex02 Commercial Website
## Date:31-10-2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
HTML CODE
```

<!DOCTYPE html>
<html>
<head>
    <title>ABC Car and Bike Showroom</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial;
            background-color: #f2f2f2;
        }

        header {
            background-color: black;
            color: white;
            text-align: center;
            padding: 25px;
        }

        nav {
            display: flex;
            justify-content: center;
            gap: 30px;
            background-color: #333;
            padding: 15px;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }

        nav a:hover {
            color: orange;
        }

        .home {
            text-align: center;
            padding: 60px;
            background-color: #ddd;
        }

        h2 {
            text-align: center;
            margin: 25px;
        }

        .container {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 25px;
            padding: 20px;
        }

        .card {
            background-color: white;
            width: 280px;
            padding: 15px;
            text-align: center;
            border-radius: 10px;
            box-shadow: 0 2px 8px gray;
        }

        .card img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            border-radius: 8px;
        }

        .card:hover {
            transform: scale(1.05);
            transition: 0.3s;
        }

        button {
            background-color: orange;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            margin-top: 10px;
            cursor: pointer;
        }

        button:hover {
            background-color: black;
        }

        footer {
            background-color: black;
            color: white;
            text-align: center;
            padding: 20px;
            line-height: 2;
        }
    </style>
</head>

<body>

    <header>
        <h1>ABC AUTOMOBILES</h1>
        <p>Your Dream Car and Bike Starts Here</p>
    </header>

    <nav>
        <a href="#home">Home</a>
        <a href="#cars">Cars</a>
        <a href="#bikes">Bikes</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
    </nav>

    <section class="home" id="home">
        <h1>Welcome to ABC Automobiles</h1>
        <p>Find Your Dream Cars and Bikes Here!</p>
        <button>Explore Now</button>
    </section>

    <h2 id="cars">OUR CARS</h2>

    <div class="container">

        <div class="card">
            <img src="https://images.unsplash.com/photo-1555215695-3004980ad54e?w=500" alt="BMW Car">
            <h3>BMW</h3>
            <p>Price: ₹50 Lakhs</p>
            <button>Buy Now</button>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1618843479313-40f8afb4b4d8?w=500" alt="Mercedes Car">
            <h3>Mercedes Benz</h3>
            <p>Price: ₹60 Lakhs</p>
            <button>Buy Now</button>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1621007947382-bb3c3994e3fb?w=500" alt="Toyota Car">
            <h3>Toyota</h3>
            <p>Price: ₹25 Lakhs</p>
            <button>Buy Now</button>
        </div>

    </div>

    <h2 id="bikes">OUR BIKES</h2>

    <div class="container">

        <div class="card">
            <img src="https://images.unsplash.com/photo-1558981806-ec527fa84c39?w=500" alt="Royal Enfield">
            <h3>Royal Enfield</h3>
            <p>Price: ₹2 Lakhs</p>
            <button>Buy Now</button>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1558981403-c5f9899a28bc?w=500" alt="Sports Bike">
            <h3>Sports Bike</h3>
            <p>Price: ₹2.5 Lakhs</p>
            <button>Buy Now</button>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1568772585407-9361f9bf3a87?w=500" alt="Yamaha Bike">
            <h3>Yamaha</h3>
            <p>Price: ₹1.8 Lakhs</p>
            <button>Buy Now</button>
        </div>

    </div>

    <section id="about">
        <h2>ABOUT US</h2>
        <p>ABC Automobiles provides the best cars and bikes
        at affordable prices with excellent customer service.</p>
    </section>

    <section id="contact">
        <h2>CONTACT US</h2>
        <p>Email: abcautomobiles@gmail.com</p>
        <p>Phone: 9876543210</p>
    </section>

    <footer>
        <p>Instagram | Facebook | YouTube</p>
        <p>© 2026 ABC Automobiles. All Rights Reserved.</p>
    </footer>

</body>
</html>

```
CSS CODE 
```

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f2f2f2;
    color: #333;
}

/* HEADER */
header {
    background-color: #151515;
    color: white;
    text-align: center;
    padding: 25px;
}

/* NAVIGATION */
nav {
    display: flex;
    justify-content: center;
    gap: 30px;
    background-color: #333;
    padding: 15px;
}

nav a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

nav a:hover {
    color: orange;
}

/* HOME */
.home {
    background-color: #ddd;
    text-align: center;
    padding: 60px;
}

/* SECTIONS */
section {
    padding: 30px;
    text-align: center;
}

h2 {
    margin-bottom: 20px;
}

/* FLEXBOX */
.container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 25px;
}

/* PRODUCT CARDS */
.card {
    background-color: white;
    width: 250px;
    padding: 15px;
    border-radius: 10px;
    box-shadow: 0 2px 8px gray;
}

.card img {
    width: 100%;
    height: 150px;
    object-fit: cover;
    border-radius: 5px;
}

.card:hover {
    transform: scale(1.05);
    transition: 0.3s;
}

/* BUTTON */
button {
    background-color: #e65c00;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    margin-top: 10px;
    cursor: pointer;
}

button:hover {
    background-color: black;
}

/* FOOTER */
footer {
    background-color: #151515;
    color: white;
    text-align: center;
    padding: 20px;
    line-height: 2;
}
```
## OUTPUT
![alt text](<Screenshot 2026-11-03 151721.png>)

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
