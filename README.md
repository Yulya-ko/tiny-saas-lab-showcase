# Tiny SaaS Lab

<div align="center">
  <h1>Tiny SaaS Lab</h1>
  <p><strong>Copy. Paste. Launch Faster.</strong></p>
  <p>A library of reusable React components and landing page building blocks for SaaS projects.</p>
  <p>
    <a href="https://tiny-saas-lab.vercel.app/">Live Demo</a> ·
    <a href="https://github.com/Yulya-ko">GitHub Profile</a>
  </p>
</div>

---

## Product Preview

<!-- Replace these image paths with your screenshots. -->
<p align="center">
  <img src="screenshots/product-overview.png" alt="Tiny SaaS Lab — product overview" width="100%" />
</p>

<p align="center">
  <em>Explore reusable UI building blocks and create landing pages faster.</em>
</p>

## About the Project

Tiny SaaS Lab is an independent product project designed to help developers build SaaS landing pages faster with reusable React components and ready-to-use UI sections.

The platform combines an interactive component catalog, responsive previews, copy-ready code for free components, premium content, and paid Collections.

## Key Features

- **Reusable Components** — Browse UI building blocks for SaaS landing pages.
- **Interactive Previews** — Explore components before using them in a project.
- **Responsive Preview Modes** — Check how components look across different screen sizes.
- **Search and Filtering** — Find components by category and other available filters.
- **FREE and PRO Access** — Explore free components and access premium content through purchases.
- **Collections** — Discover coordinated sets of landing page sections.
- **User Authentication** — Sign in and access your purchased products.
- **My Library** — Manage access to purchased content.
- **Secure Digital Delivery** — Premium source code and Collection downloads are protected by server-side authorization.
- **Payment Integration** — Purchase processing and access management are integrated with Paddle.

## Screenshots

<!--
Add your screenshots to the screenshots/ folder.
Keep the filenames below, or update the paths to match your files.
-->

### 1. Components Catalog

<p align="center">
  <img src="screenshots/components-catalog.png" alt="Components catalog with search, filters, and component cards" width="100%" />
</p>

*Browse components, explore available options, and find suitable building blocks for your project.*

### 2. Interactive Component Preview

<p align="center">
  <img src="screenshots/responsive-preview.png" alt="Interactive component preview with responsive device modes" width="100%" />
</p>

*Preview UI components before integrating them into a website.*

### 3. Collections

<p align="center">
  <img src="screenshots/collection-preview.png" alt="Tiny SaaS Lab Collection preview" width="100%" />
</p>

*Explore coordinated sets of components designed around a specific website concept.*

### 4. Customer Library

<p align="center">
  <img src="screenshots/my-library.png" alt="Customer library with purchased products" width="100%" />
</p>

*Access purchased products through a personal library.*

## My Role

I developed Tiny SaaS Lab as an independent product project, working on the frontend, application architecture, and backend integrations.

My work includes:

- Building interfaces and reusable components with React and TypeScript.
- Implementing the component catalog, search, filtering, and interactive previews.
- Developing responsive layouts and copy-code interactions.
- Integrating Supabase authentication and database functionality.
- Implementing payment flows and purchase confirmation through Paddle webhooks.
- Building server-side access control for premium content and Collection downloads.
- Handling product access based on purchases and ownership.
- Configuring deployment and maintaining separate frontend and backend workflows.

## Engineering Highlights

### Server-Side Payment Processing

Trusted product and pricing information is resolved on the server rather than accepted directly from client input.

### Webhook-Based Purchase Confirmation

The application uses signed payment webhooks to verify transactions and update purchase records before granting premium access.

### Protected Premium Content

Access to premium source code and downloadable Collections is checked on the server, helping prevent unauthorized access to paid products.

### Reusable Product Architecture

Shared catalog definitions help maintain consistency across component metadata, Collections, and product configuration.

## Tech Stack

<table>
  <tr>
    <td><strong>Frontend</strong></td>
    <td>React 19, TypeScript, Vite, Tailwind CSS, React Router</td>
  </tr>
  <tr>
    <td><strong>Backend</strong></td>
    <td>Supabase Auth, PostgreSQL, Row Level Security, Edge Functions, Storage</td>
  </tr>
  <tr>
    <td><strong>Payments</strong></td>
    <td>Paddle.js, Paddle Billing API, signed webhooks</td>
  </tr>
  <tr>
    <td><strong>Deployment & Tools</strong></td>
    <td>Vercel, Supabase CLI, ESLint, TypeScript</td>
  </tr>
</table>

## Architecture Overview

<pre>
React + TypeScript Frontend
          |
          +---- Supabase Authentication
          |
          +---- Supabase Edge Functions
          |          |
          |          +---- Server-side checkout
          |          +---- Premium access control
          |          +---- Collection downloads
          |
          +---- Paddle Checkout
                       |
                       v
                Signed Webhooks
                       |
                       v
              Purchase Records
              and Access Rights
</pre>

The frontend and backend are deployed independently. Payment verification, purchase records, access control, and private content delivery are handled through backend services.

## Validation

The project's local validation commands include:

```bash
npm run lint
npx tsc -b
npm run build
```

Payment and access-control changes also require appropriate Sandbox testing and manual integration checks.

## Project Status

Tiny SaaS Lab is an evolving product with reusable components, premium Collections, and purchase-protected digital content.

## Repository Scope

This repository is a **public project showcase**, not the application source repository.

It contains project information and selected screenshots for demonstration purposes. Proprietary component source code, paid Collection projects, credentials, environment variables, production secrets, and private artifacts are intentionally excluded.

---

<p align="center">
  <strong>Tiny SaaS Lab</strong><br />
  <em>Reusable UI building blocks for faster SaaS development.</em>
</p>
