# Catalogue

A product catalogue web application that interfaces with a WooCommerce store to display and browse sports wear products.

## Features

- Product browsing and catalog display
- WooCommerce API proxy for product data
- Image proxy for optimized image delivery
- Responsive design
- Health check endpoint

## Tech Stack

| Component | Technology |
|-----------|-----------|
| Frontend | React, TypeScript |
| Backend | Node.js, Express |
| Build Tool | Vite |
| Deployment | Vercel |

## Project Structure

```
catalogue/
├── artifacts/
│   ├── api-server/        # Express backend API
│   │   └── src/
│   │       ├── routes/    # API route handlers
│   │       └── middlewares/
│   ├── static-site/       # React frontend
│   │   └── src/
│   │       ├── components/
│   │       ├── hooks/
│   │       └── pages/
│   └── mockup-sandbox/
├── api/
│   ├── wc.js              # WooCommerce API proxy (Vercel serverless)
│   └── img-proxy.js       # Image proxy (Vercel serverless)
├── lib/
│   ├── db/                # Database schema (Drizzle ORM)
│   ├── api-client-react/  # API client hooks
│   ├── api-spec/          # API specification
│   └── api-zod/           # Zod validation schemas
├── server.js              # Express server (local development)
├── package.json
├── tsconfig.json
└── vercel.json
```

## Getting Started

### Prerequisites
- Node.js 18+
- pnpm

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/arooba-shafique/catalogue.git
   cd catalogue
   ```

2. Install dependencies:
   ```bash
   pnpm install
   ```

3. Start the development server:
   ```bash
   node server.js
   ```

4. Open `http://localhost:3000` in your browser.
