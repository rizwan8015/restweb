# Ex.06 Restaurant Website
## Date: 12-11-2024

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
### HTML Code:
```html
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Little Lemon Restaurant</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="background"></div>

    <nav class="navbar">
        <div class="logo">Little Lemon Restaurant</div>
        <img src="Images/Asset 7@4x.png" alt="">
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#menu">Menu</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <div class="bg">
        <div class="menu-container">
            <div class="card">
                <img src="https://images.pexels.com/photos/5560763/pexels-photo-5560763.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Dosa">
                <div class="card-content">
                    <h3>Dosa</h3>
                    <p>Crispy and Yummy Dosa.</p>
                    <span class="price">Rs. 30</span>
                </div>
            </div>
            
            <div class="card">
                <img src="https://images.pexels.com/photos/28674705/pexels-photo-28674705/free-photo-of-indian-dal-and-rice-in-traditional-utensils.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Dal Rice">
                <div class="card-content">
                    <h3>Dal Rice</h3>
                    <p>Traditional Indian Dal and Rice.</p>
                    <span class="price">Rs. 50</span>
                </div>
            </div>
        
            <div class="card">
                <img src="https://images.pexels.com/photos/20422135/pexels-photo-20422135/free-photo-of-meal-on-plate-and-sauces.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Vada">
                <div class="card-content">
                    <h3>Vada</h3>
                    <p>Crispy and Crunchy Vada.</p>
                    <span class="price">Rs. 10</span>
                </div>
            </div>
        </div>
        <div class="menu-container">
            <div class="card">
                <img src="https://images.pexels.com/photos/29333631/pexels-photo-29333631/free-photo-of-warm-ceramic-coffee-cup-on-marble-surface.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Coffee">
                <div class="card-content">
                    <h3>Coffee</h3>
                    <p>A delightful Coffee.</p>
                    <span class="price">Rs. 10</span>
                </div>
            </div>
            
            <div class="card">
                <img src="https://images.pexels.com/photos/20689160/pexels-photo-20689160/free-photo-of-flat-bread-and-elephant-figurine.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Chappathi">
                <div class="card-content">
                    <h3>Chappathi</h3>
                    <p>Soft Chapathi.</p>
                    <span class="price">Rs. 15</span>
                </div>
            </div>
        
            <div class="card">
                <img src="https://images.pexels.com/photos/2456435/pexels-photo-2456435.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Noodles">
                <div class="card-content">
                    <h3>Noodles</h3>
                    <p>Nice and long Noodles.</p>
                    <span class="price">Rs. 100</span>
                </div>
            </div>
        </div>
    </div>
    
</body>
</html>
```

### CSS Code:
```css
@import url('https://fonts.googleapis.com/css2?family=Delius&family=Pacifico&family=Quicksand:wght@300..700&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: "Quicksand", sans-serif;
    font-optical-sizing: auto;
    font-weight: 10;
    font-style: bold;
}

.background {
    position: fixed;
    inset: 0;
    background-image: url("https://wallpaperboat.com/wp-content/uploads/2020/02/table-03.jpg");
    background-size: cover;
    background-position: center;
    z-index: -1;
    filter: blur(4px);
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #FFC20D;
    padding: 10px 20px;
}

.navbar img{
    display: flex;
    height: 70px;
    width: 40px;
}

.navbar .logo {
    color: #028940;
    font-size: 3em;
    font-weight: bold;
}

.nav-links {
    list-style: none;
    display: flex;
    gap: 15px;
}

.nav-links li {
    display: inline;
    font-size: 1.5em;
}

.nav-links a {
    color: green;
    text-decoration: none;
    padding: 8px 15px;
    transition: background 0.3s;
}

.nav-links a:hover {
    background-color: #ffffffbe;
    border-radius: 4px;
}

.menu-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    padding: 20px;
    margin-top: 60px;
    justify-content: center;
}

.card {
    background-color: white;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    overflow: hidden;
    width: 300px;
    transition: transform 0.3s;
}

.card:hover {
    transform: scale(1.05);
}

.card img {
    width: 100%;
    height: 150px;
    object-fit: cover;
}

.card-content {
    padding: 15px;
    text-align: center;
}

.card-content h3 {
    font-size: 1.25em;
    margin-bottom: 10px;
    color: #333;
}

.card-content p {
    font-size: 0.9em;
    color: #777;
    margin-bottom: 10px;
}

.price {
    display: block;
    font-size: 1.1em;
    font-weight: bold;
    color: #e67e22;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/fbc242c0-1d08-4d87-b391-821b0d0aba60)


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
