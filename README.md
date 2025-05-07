# Lost Saga REST API Monorepo

This repository contains multiple backend and frontend projects for Lost Saga, including a REST API built with [Hono](https://hono.dev/) (TypeScript), and Next.js API implementations in both JavaScript and TypeScript. The APIs provide endpoints for authentication, billing, launcher logic, and more, with strong validation and modular design.

---

## Table of Contents

- [Lost Saga REST API Monorepo](#lost-saga-rest-api-monorepo)
  - [Table of Contents](#table-of-contents)
  - [Projects](#projects)
    - [1. `with-hono`](#1-with-hono)
    - [2. `withNextJS`](#2-withnextjs)
  - [Project Structure](#project-structure)
  - [Getting Started](#getting-started)
  - [API Overview](#api-overview)
  - [Contributing](#contributing)
  - [License](#license)

---

## Projects

### 1. `with-hono`

A REST API backend using Hono (TypeScript). Features modular routing, strong validation (Zod), custom SEED encryption, and endpoints for billing and launcher logic.

- See [`with-hono/README.md`](./with-hono/README.md) for full details and API documentation.

### 2. `withNextJS`

Contains two Next.js API implementations:

- `losaapi-js`: Next.js API routes in JavaScript.
- `losaapi-ts`: Next.js API routes in TypeScript with ESLint.

Each provides endpoints for user authentication, cash management, and payment logic.

- See [`withNextJS/losaapi-js/README.md`](./withNextJS/losaapi-js/README.md) and [`withNextJS/losaapi-ts/README.md`](./withNextJS/losaapi-ts/README.md) for usage and configuration.

---

## Project Structure

```
rest-api/
├── with-hono/         # Hono REST API (TypeScript)
├── withNextJS/
│   ├── losaapi-js/    # Next.js API (JavaScript)
│   └── losaapi-ts/    # Next.js API (TypeScript)
└── README.md          # Main monorepo README
```

---

## Getting Started

1. **Clone the repository:**

   ```bash
   git clone https://github.com/LSFDC/ls-rest-api.git
   cd rest-api
   ```

2. **Install dependencies for each project:**

   ```bash
   cd with-hono
   npm install
   # or
   cd ../withNextJS/losaapi-js
   npm install
   # or
   cd ../losaapi-ts
   npm install
   ```

3. **Configure environment variables:**

   - Each project may require database and environment configuration. See the respective `README.md` files for details.

4. **Run the development server:**
   ```bash
   npm run dev
   ```

---

## API Overview

- **Billing:** Endpoints for getting user cash, making payments, and gifting.
- **Launcher:** Endpoints for user authentication and game launcher initialization.
- **Encryption:** Uses SEED cipher (CFB mode) for sensitive data.
- **Validation:** Strong input validation using Zod (Hono) or manual checks (Next.js).

See each project’s README for detailed API documentation and example requests.

---

## Contributing

Contributions, bug reports, and feature requests are welcome! Please open an issue or submit a pull request.

---

## License

This repository is licensed under the [MIT License](./LICENSE).

---
