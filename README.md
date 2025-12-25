🍔 FoodFlow - Modern Food Delivery SPA
A high-performance, responsive food delivery Single Page Application (SPA) built with a focus on clean architecture, smooth animations, and a mobile-first User Interface.

Built using React and Tailwind CSS directly in the browser, requiring no build steps or installation.
An app photo app
![2E418314-5D5F-41AD-A343-FDD5FE6AA1F6](https://github.com/user-attachments/assets/ebea8c4b-c495-4e01-a0dd-b442bc464332)
![FE7AE7B3-C7BD-430D-938B-B5BEC8AEBF1B](https://github.com/user-attachments/assets/53f77b66-518c-4777-8903-8d67b6042bdf)
![EE775608-C3C9-4320-92F7-0DAF2995FAEC](https://github.com/user-attachments/assets/1fba2f73-1198-47e9-8eca-800b47112f11)
A![A365AC27-A6EF-4251-9D15-54E7828DFBDE](https://github.com/user-attachments/assets/55e77257-e5a6-4f9f-98c0-eba1e5e26c20)


FoodFlow DemoReactTailwind

✨ Features
🔍 Dynamic Filtering: Filter restaurants by category (Burger, Sushi, Pizza, Mexican, Healthy) with smooth transitions.
🍕 Expanded Menus: Each restaurant features a unique menu with 8 distinct food items.
🛒 Functional Cart System:
Add items to the basket.
Adjust quantities (+ / -).
Automatic calculation of subtotal, delivery fees, and total.
Logic to prevent mixing items from different restaurants without confirmation.
🎨 Premium UI/UX:
Real Photos: High-quality Unsplash images for all food items.
Animations: Skeleton loading states, staggered entry animations, cart slide-up sheets, and toast notifications.
Glassmorphism: Backdrop blur effects in headers and overlays.
🚀 Zero Configuration: No node_modules, no npm install. Just open the HTML file.
🛠 Tech Stack
Frontend: React 18 (via CDN)
Transpiler: Babel (via CDN)
Styling: Tailwind CSS (via CDN)
State Management: React Context API (Zustand-like pattern)
Icons: Custom SVG Components
Fonts: Plus Jakarta Sans
📂 Project Architecture
The application follows a clean architecture pattern, separating concerns within the single-file structure:

Data Layer: RESTAURANTS constant acting as the Mock API database.
State Layer: CartProvider (Context) managing global cart state, logic, and persistence.
UI Layer: Functional Components (Header, CartSheet, Home, Detail) focused solely on rendering and user interaction.
Hooks: Custom logic for managing state updates and side-effects.
🚀 How to Run
Since this project is built as a standalone HTML file with CDN links, setup is instant.

Download/Copy the index.html code provided.
Save it to your computer as index.html.
Open the file in any modern web browser (Chrome, Edge, Firefox, Safari).
Enjoy! No server or internet connection is strictly required after the first load (except for loading the images).
📱 Screens & Flow
Home Screen:
Displays a list of available restaurants.
Horizontal scrolling tabs to filter by category.
Skeleton loaders during the "simulated" API fetch.
Detail Screen:
Shows restaurant header image and details.
Scrollable list of 8 menu items with specific prices and descriptions.
"Add to Cart" button triggers the cart drawer.
Cart Drawer:
Bottom sheet UI revealing current basket.
Quantity adjustment controls.
Checkout button with total calculation.
🧩 Customization
Adding a New Restaurant
Edit the RESTAURANTS array in the <script> tag:

{  id: "r6",  name: "New Place",  rating: 4.5,  category: "NewCategory",  img: "URL_TO_IMAGE",  menu: [     // Add items here  ]}
Changing Colors
Search for the --primary: #FF6B6B style in the <style> section to change the brand accent color.

🐛 Known Limitations
Single File: All code resides in one file. For production, this should be split into components.
No Backend: Data is currently mocked in the JavaScript file.
Persistence: Cart state clears upon page refresh (could be added with localStorage easily).
📝 License
This project is open source and available for educational purposes.

