Restaurant Website - Foodie
A modern, responsive restaurant website with online food ordering system built with HTML, CSS, and JavaScript.
🍕 Features

Home Page - Attractive landing page with hero carousel showcasing restaurant offerings
Menu Page - Comprehensive menu with category filters (Pizza, Burger, Pasta, Fries)
About Page - Information about the restaurant
Book Table - Table reservation system with integrated Google Maps
Online Ordering System - Complete food ordering experience with:

Shopping cart functionality
Category-based filtering
Add/remove items with quantity controls
Multi-step checkout process
Multiple payment options
Order confirmation



📁 File Structure
restaurant-website/
│
├── index.html          # Homepage with carousel and featured sections
├── menu.html           # Full menu page with filtering
├── about.html          # About the restaurant
├── book.html           # Table booking page
├── order.html          # Online ordering page (basic)
├── proceed.html        # Online ordering page (simplified checkout)
│
├── css/
│   ├── bootstrap.css   # Bootstrap framework
│   ├── style.css       # Custom styles
│   ├── responsive.css  # Responsive design styles
│   └── font-awesome.min.css  # Icon fonts
│
├── js/
│   ├── jquery-3.4.1.min.js
│   ├── bootstrap.js
│   └── custom.js       # Custom JavaScript
│
└── images/
    ├── hero-bg.jpg     # Hero section background
    ├── about-img.png   # About section image
    ├── favicon.png     # Site favicon
    ├── f1.png - f9.png # Food item images
    ├── o1.jpg, o2.jpg  # Offer images
    └── client1.jpg, client2.jpg  # Customer testimonial images
🚀 Getting Started
Prerequisites

Web browser (Chrome, Firefox, Safari, Edge)
Text editor (VS Code, Sublime Text, etc.) for modifications
Basic knowledge of HTML/CSS/JavaScript (for customization)

Installation

Clone or Download the repository

bashgit clone <repository-url>

Open the project in your preferred text editor
Launch the website by opening index.html in a web browser

🎨 Pages Overview
1. Homepage (index.html)

Hero carousel with call-to-action buttons
Featured offers section
Menu preview with category filtering
About section preview
Table booking form
Customer testimonials
Opening hours and contact information

2. Menu Page (menu.html)

Complete food menu
Category filters (All, Burger, Pizza, Pasta, Fries)
Individual item cards with:

Food images
Descriptions
Prices
Add to cart buttons



3. About Page (about.html)

Restaurant story and information
High-quality imagery
Contact details

4. Book Table (book.html)

Reservation form with fields:

Name
Phone number
Email
Number of persons
Date selection


Integrated Google Maps location

5. Order Online (order.html)

Full-featured ordering system with:

Sliding cart sidebar
Menu items with images and descriptions
Category filtering
Add to cart functionality
Quantity controls
Multi-step checkout modal:

Step 1: Delivery method selection (Delivery/Takeaway)
Step 2: Delivery address details
Step 3: Payment method selection
Step 4: Order summary and confirmation


Order success animation
Real-time cart total calculation



6. Proceed (proceed.html)

Simplified ordering page
Basic checkout with alert-based confirmation

🛠️ Customization Guide
Update Restaurant Information
Logo and Name:
html<!-- Find and replace "Foodie" or "Feane" with your restaurant name -->
<div class="logo">Your Restaurant Name</div>
Contact Details:
html<!-- Update in footer section -->
<span>Call +01 1234567890</span>  <!-- Your phone -->
<span>demo@gmail.com</span>        <!-- Your email -->
<span>Location</span>               <!-- Your address -->
Opening Hours:
html<p>10.00 Am -10.00 Pm</p>  <!-- Update timing -->
Add Menu Items
Edit the menuItems array in order.html:
javascriptconst menuItems = [
    {
        id: 16,
        name: 'Your Dish Name',
        price: 9.99,
        category: 'pizza', // or 'burger', 'pasta', 'fries', 'desserts'
        image: 'image-url',
        description: 'Delicious description'
    }
];
Update Colors
Primary Color (Orange/Yellow):
css/* Change #ffbe33 to your brand color throughout CSS */
background: #ffbe33;
color: #ffbe33;
border-color: #ffbe33;
Dark Theme:
css/* Change #222831 for dark elements */
background: #222831;
Add New Categories

Add filter button:

html<button class="filter-btn" onclick="filterMenu('newcategory')">New Category</button>

Add menu items with matching category
Update filtering logic if needed

📱 Responsive Design
The website is fully responsive and optimized for:

Desktop (1200px+)
Tablet (768px - 1199px)
Mobile (320px - 767px)

🔧 Technologies Used

HTML5 - Structure and content
CSS3 - Styling and animations
JavaScript (Vanilla) - Interactive functionality
Bootstrap 4 - Grid system and components
Font Awesome 6 - Icons
jQuery 3.4.1 - DOM manipulation
Owl Carousel 2 - Carousels and sliders
Isotope - Filtering and sorting
Nice Select - Custom select dropdowns
Google Maps API - Location maps

🌟 Key Features Explained
Shopping Cart System

Persistent cart during session
Add/remove items
Quantity increment/decrement
Real-time total calculation
Sliding sidebar interface

Multi-Step Checkout

Progressive disclosure design
Form validation
Delivery vs. Takeaway selection
Multiple payment options:

Cash on Delivery
Credit/Debit Card
UPI Payment
Digital Wallet


Order summary review
Success confirmation with order ID

Menu Filtering

Isotope-based filtering on static pages
JavaScript-based filtering on ordering pages
Smooth animations
Active state indicators

📝 Configuration
Google Maps API
Replace the API key in all HTML files:
html<script src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=myMap"></script>
Get your API key from Google Cloud Console
Image URLs
For order.html, images are loaded from Unsplash. For production:

Download images or use your own
Place in images/ folder
Update image paths in the menuItems array

🐛 Troubleshooting
Cart not opening:

Check browser console for JavaScript errors
Ensure all script files are loaded properly

Images not loading:

Verify image paths are correct
Check if images exist in the images/ folder
For order.html, ensure internet connection for Unsplash images

Google Maps not showing:

Verify API key is valid
Check if Maps JavaScript API is enabled in Google Cloud Console
Ensure callback function myMap exists in custom.js

🚀 Performance Tips

Optimize Images:

Compress images before uploading
Use WebP format for better compression
Implement lazy loading for below-fold images


Minimize CSS/JS:

Combine and minify CSS files
Combine and minify JavaScript files
Remove unused CSS/JS


Enable Caching:

Add cache headers on server
Use CDN for static assets



📄 License
This project uses templates from:

Free Html Templates (https://html.design/)
ThemeWagon (https://themewagon.com/)

🤝 Support
For issues or questions:

Check the troubleshooting section
Review browser console for errors
Ensure all dependencies are loaded

🔄 Future Enhancements
Potential additions:

User authentication system
Order tracking functionality
Payment gateway integration
Admin dashboard for order management
Database integration
Email notifications
Customer reviews and ratings
Loyalty program
Mobile app version


Built with ❤️ for food lovers everywhere! 🍕🍔🍝
