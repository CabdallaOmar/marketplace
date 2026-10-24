# ZAYRO E-Commerce Frontend

**Shop Smart. Live Better.**

ZAYRO is a responsive frontend-only e-commerce demonstration built with Next.js App Router, TypeScript, Tailwind CSS, React Context, and localStorage. The product catalogue, reviews, stock, and prices are sample data. Checkout, account screens, contact forms, and newsletter feedback are simulated.

## Run locally

1. Install Node.js 20.9 or later.
2. In PowerShell, install project dependencies with npm.cmd install.
3. Start the development server with npm.cmd run dev.
4. Open http://localhost:3000.

On Windows, scripts/prepare-project.ps1 installs the dependencies and checks the Unsplash image URLs.

On macOS or Linux, replace npm.cmd with npm.

Other scripts:

- npm run lint - run ESLint.
- npm run typecheck - run the TypeScript check.
- npm run build - create the production build.
- npm run profile - regenerate the company profile PDF when Python and ReportLab are installed.
- npm run verify:images - check that the external Unsplash photos respond as images.

## Pages

- / - home, product categories, featured finds, newsletter demo.
- /shop - product search, category and price filters, sorting.
- /product/[id] - product details, options, quantity, cart and wishlist actions.
- /cart - cart quantities, removal, subtotal and simulated shipping.
- /checkout - validated demo checkout; no card data or real payment.
- /order-success - local demo order confirmation.
- /wishlist - saved products.
- /account - sign-in and registration previews; no real authentication.
- /about - company concept, vision, mission, values and future plans.
- /contact - validated contact form preview; no live inbox.

## Demo behavior

- Cart, wishlist, and theme preference persist in localStorage.
- First visit follows the operating system's light/dark preference unless a theme is saved.
- Sample prices use USD, and simulated shipping is shown as a demo estimate.
- Order details are saved locally in the browser to display the confirmation page.
- No backend, database, payment processing, real authentication, fulfilment, or email delivery is connected.

## Brand and photography

The supplied ZAYRO logo is in public/zyro-removebg-preview.jpg. It is used in the header, footer, browser icon, and Company Profile cover.

Product and lifestyle photos load from Unsplash's image CDN. The site needs an internet connection to display them. Source searches and the license link are listed in docs/IMAGE_SOURCES.md. A fallback photo is configured for load errors. Review the current license terms before production use.

## Project documents

- Business Idea: docs/ZAYRO_Business_Idea.md
- Photography sources: docs/IMAGE_SOURCES.md
- Company Profile PDF: output/pdf/ZAYRO_Company_Profile.pdf

The PDF generator is scripts/generate_company_profile.py. The profile avoids unprovided contact details and clearly labels future services as plans.
