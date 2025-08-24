My personal portfolio website, built with HTML, Tailwind CSS, and JavaScript. It features a clean, modern design to showcase my skills and projects as a Cyber Security Specialist and Web Developer.
1. Setting Up the Basic Structure (HTML)
The foundation is a single HTML file (index.html). The structure is semantic and straightforward:

<head>: This is where you link all the necessary files and libraries.

Tailwind CSS: For all the styling. It's linked via a CDN, which is the easiest way to start.

Google Fonts: The "Inter" font is imported for a clean, modern look.

Lucide Icons: For the social media and menu icons.

<body>: This contains the main content, divided into logical sections:

<header>: The navigation bar that stays fixed at the top of the page.

<main>: The core content, with each part of your portfolio in its own <section> tag (Home, About, Skills, Projects, Contact).

<footer>: The simple footer at the bottom.

<script> tags: At the very end of the body, we include the JavaScript libraries and our custom script.

2. Styling with Tailwind CSS
Instead of writing traditional CSS, this portfolio uses Tailwind CSS. It's a "utility-first" framework, which means you build the design directly in your HTML using pre-made classes.

Layout: Classes like flex, grid, container, mx-auto are used to structure the page and center the content.

Colors & Spacing: The dark theme is created with classes like bg-[#111111] (for the background) and text-[#A3A3A3] (for the text). The green accent color comes from accent-green and bg-accent-green, which are custom classes defined in the <style> block. Spacing is controlled with classes like p-8 (padding) and mb-12 (margin-bottom).

Cards: The stylish cards for your skills and projects are made by combining classes: card-bg, border-card, and rounded-lg.

3. Adding Interactivity (JavaScript)
This is where the portfolio comes to life. There are a few key JavaScript parts:

Mobile Menu: A simple script listens for a click on the menu button and toggles the hidden class on the mobile menu div to show or hide it.

Scroll Animations: The "fade-in" effect on sections as you scroll is handled by the IntersectionObserver API. It's a modern way to detect when an element enters the screen and then add a .visible class to trigger the animation defined in the CSS.

Glowing Cursor: A div with the ID cursor-glow is created. A mousemove event listener tracks the mouse's position and updates the left and top properties of the div, making it follow the cursor.

Animated Headline: The main headline text is split into individual characters. Each character is wrapped in a <span> with a staggered animation-delay, which makes them fade in one by one.

3D Tilt Effect: This is the coolest part! It's powered by an external library called vanilla-tilt.js.

It's included with a <script> tag at the bottom.

Any element that you want to have the tilt effect just needs the data-tilt attribute added to it in the HTML.

A small script at the end initializes the library on all elements with that attribute.

By combining these three layers—HTML structure, Tailwind CSS for styling, and JavaScript for interactivity—you get a professional and dynamic portfolio.
