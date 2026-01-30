<img src="https://res.cloudinary.com/dtl48kr1u/image/upload/v1694116269/fake-shop/logo2_drwmph.png" width="120" alt="Squisito" />

Squisito is a Next.js e-commerce-style app for kitchen appliances (fake shop). It lists products from MongoDB, supports product detail pages, cart, and checkout. The brand logo is used in the navbar and footer.

## Composition

The app is built around a small storefront flow:

- **Home**: featured products and entry to catalog.
- **Products**: product listing and filters.
- **Product detail**: single product page with variants (e.g. colours).
- **Cart** and **Checkout**: cart context and checkout page.

## Features

- Products and details loaded from MongoDB via `/api/get-products` and `/api/product-by-id`.
- Cart state via `CartContext`; product data via `ProductContext`.
- NavBar and Footer use the Squisito logo (e.g. `logo2` from Cloudinary or local `Images`).
- Product images by variant (e.g. colour) in `public/Images/`.
- Favicon: `public/Images/Icons/favicon.png`.
- MUI, FontAwesome, Bootstrap for UI.

## Technology

- Next.js 13 + React 18
- TypeScript
- MongoDB
- MUI (Material-UI), FontAwesome, Bootstrap
- Emotion

## Setup

```bash
npm install
npm run dev
```

Configure MongoDB connection (e.g. env var used in `lib/mongodb.ts` and API routes).

Open [http://localhost:3000](http://localhost:3000).

## Build

```bash
npm run build
npm run start
```

## Logo

- **Logo**: The image above is the app logo (Cloudinary: `fake-shop/logo2_drwmph.png`). Used in `NavBar` and `Footer`.
- **Favicon**: `public/Images/Icons/favicon.png`.

## Notes

- This is a fake shop; no real payments.
- Media folder at repo level (e.g. Loader, Logo, Products) is for design/assets; Logo folder contains the brand logos to keep.
