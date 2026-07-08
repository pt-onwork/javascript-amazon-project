# JavaScript Amazon Project

A front-end clone of Amazon's shopping experience, built with vanilla JavaScript, HTML, and CSS — covering the full flow from browsing products to checkout, order placement, and delivery tracking.

## Features

- **Home / Product Listing (`amazon.html`)** – Browse products loaded from a local data set, with product images, ratings, pricing, and quantity selectors.
- **Shopping Cart** – Add products to the cart, update quantities, and remove items, with cart state persisted so it survives page reloads.
- **Checkout (`checkout.html`)** – Review cart items, choose a delivery option/date for each product, and see order totals calculated dynamically (subtotal, shipping, tax, total).
- **Order Placement & History (`orders.html`)** – Place an order and view a history of past orders with their items and dates.
- **Delivery Tracking (`tracking.html`)** – Track the delivery progress of a placed order with a visual progress bar.
- **Backend** – A local backend (in `backend/`) used to persist cart and order data during development/testing.
- **Automated Tests (`tests/`)** – Unit tests covering cart and checkout logic.

## Project Structure
```
javascript-amazon-project/
├── amazon.html          # Home page — product listing
├── checkout.html         # Cart review & delivery options
├── orders.html            # Order history
├── tracking.html           # Order delivery tracking
├── backend/                # Local backend for cart/order persistence
├── data/                    # Product and order data
├── images/                  # Product and UI images/icons
├── scripts/                 # JavaScript logic (cart, checkout, orders, utils, etc.)
├── styles/                  # CSS stylesheets
├── tests/                   # Unit tests
└── notes.txt                 # Personal learning notes
```
## Tech Stack

- **Languages:** JavaScript (87.5%), CSS (9.3%), HTML (3.2%)
- No frameworks — built with plain JavaScript (DOM manipulation, ES modules, `data-*` attributes, `localStorage`/backend persistence)

## Getting Started

1. Clone the repository:
```bash
   git clone https://github.com/pt-onwork/javascript-amazon-project.git
   cd javascript-amazon-project
```

2. If the project uses the local backend (check the `backend/` folder for setup instructions, e.g. a `package.json` or server script), start it first:
```bash
   cd backend
   npm install
   npm start
```

3. Serve the frontend with any static file server (opening `amazon.html` directly may cause issues with modules or the backend connection):
```bash
   npx serve .
```

4. Open `amazon.html` in your browser to start browsing, then proceed through checkout, orders, and tracking.

## Running Tests

Check the `tests/` folder for the test runner used (e.g. Jasmine). Typically:
```bash
npx jasmine
```
or open the provided test runner HTML file in a browser if one is included.

## About This Project

This project was built as a hands-on exercise in core JavaScript concepts — DOM manipulation, `data-*` attributes, event handling, dynamic rendering, and working with a simple backend for persistence — while recreating a real-world e-commerce flow.

## License

No license specified yet. Consider adding one (e.g. MIT) if you plan to share or open-source this project.
