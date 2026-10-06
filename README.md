# my3dshop
3d print shop is a single-page front-end demo for a 3D-printing storefront. It combines HTML, CSS, and JavaScript in one file and uses Three.js to display interactive 3D objects.

Features
Product catalog with search, category filters, and sorting
Product details with an interactive 3D viewer
Theme options, including dark, light, neon, and retro styles
Shopping cart, wishlist, promo codes, and simulated checkout
Custom-print quote interface for .stl files
Material guide for PLA, PETG, resin, TPU, and nylon
Product quiz, mini-game, rewards, achievements, and daily spin
Responsive layout for desktop and smaller screens
Printy help widget with predefined answers
Browser-local storage for demo cart, wishlist, and reward data
How to Run
Save the HTML source as index.html.
Open index.html in a modern browser.
Make sure you have an internet connection if the page loads Three.js or fonts from a CDN.
If the 3D viewer does not load when opening the file directly, try running a local web server from the folder containing index.html:

python -m http.server 8000
Then open http://localhost:8000 in your browser.

How the Code Is Organized
HTML: page sections, navigation, product cards, dialogs, and forms.
CSS: layout, responsive behavior, themes, animations, and visual styling.
JavaScript: product data, filters, cart behavior, the 3D viewer, custom-print quote calculations, quiz, rewards, and other interactions.
Three.js: creates and displays procedural 3D shapes in the browser.
localStorage: saves selected demo data in the current browser.
Editing Products
Look for the JavaScript product array named P. Product entries contain details such as the product name, category, price, shape, description, rating, stock, print time, layer height, infill, and weight. Edit those values to change the demo catalog.

Important Limitations
This is a front-end demo, not a production-ready online store.

Checkout is simulated; no real payment is processed.
Product, cart, wishlist, and reward behavior is handled in the browser.
The custom-print flow uses an .stl file locally for the demo; it does not provide a complete secure upload and manufacturing pipeline.
Printy uses predefined responses; it is not a live AI assistant.
Order tracking, shipping, and fulfillment are not connected to a real backend.
Data saved with localStorage is specific to the browser and device and is not a shared customer database.
Before Launching a Real Store
A production version would need a secure backend and database, user accounts if required, secure file storage and validation, a payment provider, real order management, shipping integration, and privacy/security testing. Never put secret API keys or payment credentials in client-side HTML or JavaScript.

Technologies
HTML
CSS
JavaScript
Three.js
Browser localStorage
License
No license information was included with the source. Add a license before distributing the project if needed.
