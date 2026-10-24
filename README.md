
# STILL — Room for Living

STILL is a minimalist furniture storefront concept. It combines a clean editorial layout with an interactive 3D living room, a product catalogue, category filters, and a demo shopping bag.

> **Project Status:** Front-end prototype. Products, names, and prices are illustrative examples. Checkout and payment processing are not connected to a transaction service.

## Features

- Responsive minimalist design for desktop and mobile devices.
- Interactive 3D living room built with Three.js.
- 3D camera controls for exploring the room.
- Camera reset functionality.
- Two room themes: Warm Natural and Soft Stone.
- Interactive furniture hotspots with product details.
- Product catalogue featuring Seating, Tables, and Lighting.
- Category filters for browsing products.
- Demo shopping bag with add, remove, and quantity adjustment features.
- Automatic subtotal calculation.
- Local shopping bag persistence using `localStorage`.
- Fallback messages for unavailable product images.
- Basic accessibility support, including keyboard focus indicators and ARIA attributes.
- Reduced-motion support for users who prefer fewer animations.

## Technologies

- HTML5
- CSS3
- JavaScript ES Modules
- [Three.js](https://threejs.org/)
- OrbitControls
- RoundedBoxGeometry
- jsDelivr CDN

No build tools or front-end frameworks are required for the current prototype.

## Getting Started

### 1. Prepare the Project

Save the main HTML file as:

```text
index.html
```

### 2. Run the Project

Open `index.html` in a modern web browser.

For more reliable support of JavaScript modules, use a local development server.

If Python is installed, run the following command from the project directory:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

An internet connection is required to load Three.js modules and external product images.

## Project Structure

```text
still-store/
├── index.html
└── README.md
```

The current implementation contains the HTML, CSS, JavaScript, product data, shopping bag logic, and 3D scene in a single HTML file.

As the project grows, these components can be separated into dedicated folders for easier maintenance.

## How to Use

1. Browse the product catalogue or select **The 3D Room** from the navigation.
2. Drag the mouse or swipe to explore the 3D room.
3. Hover over or tap a furniture hotspot to view product details.
4. Select **Warm Natural** or **Soft Stone** to change the room's appearance.
5. Use the plus button on a product card or the **Add to bag** button to add a product.
6. Open **Bag** to adjust product quantities or remove items.
7. Use the **Seating**, **Tables**, and **Lighting** filters to browse specific categories.
8. Use the camera reset button to restore the initial 3D view.

## Product Data and Images

Sample product data is defined in the JavaScript section of `index.html`.

Each product contains:

- Product ID
- Product name
- Category
- Illustrative price in USD
- Finish description
- Product image URL
- Reference photo source URL

Product images are loaded from external websites and require an internet connection.

Before publishing the website, replace reference images with properly licensed or authorised product photography.

## Current Limitations

- This is a front-end prototype, not a production-ready online store.
- Product names and prices are illustrative.
- Checkout is a demonstration only; no payments are processed.
- No backend or product database is connected.
- User authentication and inventory management are not implemented.
- Shipping and order management are not implemented.
- Shopping bag data is stored locally in the browser and is not synchronised across devices.
- The 3D room requires browser support for WebGL.
- External images and dependencies may become unavailable.

## Future Improvements

- Separate HTML, CSS, and JavaScript into maintainable modules.
- Connect product data to an API or database.
- Implement backend services for shopping bags and orders.
- Add inventory and user account management.
- Integrate a secure payment provider.
- Add automated tests for product filters, shopping bag operations, and 3D hotspots.
- Optimise images and improve performance on mobile devices.
- Improve accessibility and fallback support for browsers without WebGL.

## Licence and Attribution

This project does not define a licence for the source code or third-party assets.

Review the applicable licences for dependencies, product photography, and other external resources before distributing the project or using it commercially.

---

**STILL — Room for Living**  
*A quieter kind of home.*
