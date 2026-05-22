# ShopHub

An Amazon-inspired ecommerce frontend built with React, Vite, Tailwind CSS, and DaisyUI.  
This project focuses on reusable components, multi-page routing, local authentication, cart flow, product reviews, support chat, and profile customization.

## Live Project

`Live Link:` [ShopHub](https://shop-hub-opal.vercel.app/) 




## Project Snapshot

ShopHub is a modern ecommerce practice project where users can:

- browse products and deals
- open product details pages
- add items to cart
- complete a checkout flow
- create an account and sign in
- upload a profile image
- chat with support
- write text reviews on products

The project is built as a learning-focused storefront with reusable UI and shared state across pages.

## Core Features

- Responsive homepage with banner carousel, categories, feature strip, and product sections
- Dedicated pages for products, deals, product details, cart, checkout, contact, and account
- Local auth flow with Sign In, Sign Up, AuthLayout, and private routes
- Demo captcha checkbox using an `I am not a robot` interaction
- Reusable cart system with quantity updates and order summary
- Product review section with text comments from signed-in users
- Support chat section with stored local conversation history
- Profile image upload with preview and navbar avatar integration
- Vercel SPA rewrite support through `vercel.json`

## Pages Included

- `/` Home
- `/products` Products page
- `/products/:id` Product details page
- `/deals` Deals page
- `/cart` Cart page
- `/checkout` Checkout page
- `/contact` Contact page
- `/account` Account page
- `/auth/signin` Sign in page
- `/auth/signup` Sign up page

## Tech Stack

- React
- Vite
- React Router DOM
- Tailwind CSS
- DaisyUI
- React Icons
- LocalStorage for demo persistence

## Reusable Structure

This project uses reusable shared pieces to keep the UI scalable:

- shared product card
- shared section header
- cart summary component
- quantity control component
- fake captcha component
- support chat component
- review section component
- route guard with private route

It also uses shared context providers for:

- authentication
- shopping cart and product state
- community data like reviews and chat messages

## What I Learned

While building this project, I learned and practiced:

- how to create a multi-page React application using React Router
- how to design reusable components instead of repeating the same UI
- how to manage shared app state with Context API
- how to protect routes with authentication logic
- how to create Sign In and Sign Up flows in a frontend project
- how to store user, cart, chat, and review data in `localStorage`
- how to create a product details page from dynamic route params
- how to build cart and checkout flow in an ecommerce UI
- how to add user-generated text reviews and comment sections
- how to create a simple support chat experience
- how to handle image uploading with `FileReader`
- how to make a React project responsive with Tailwind CSS and DaisyUI
- how to prepare a Vercel deployment for a single-page application

## Local Demo Notes

This project currently uses demo frontend-only logic for:

- authentication
- captcha
- chat
- reviews
- profile image upload

That means the project is great for learning and portfolio presentation, but it is not a production-ready backend system yet.

## Future Improvement Ideas

- connect real backend authentication such as Firebase or Auth0
- use real Google reCAPTCHA
- save cart and reviews in a database
- add payment gateway integration
- add wishlist and order history
- add product search and advanced filters
- add admin dashboard for product and review management

## Installation

```bash
npm install
npm run dev
```

## Build For Production

```bash
npm run build
npm run preview
```

## Deployment Note

This project includes a `vercel.json` rewrite rule so React Router pages work correctly after deployment on Vercel.

## Author Note

This project was built as a practical learning journey in modern React ecommerce development.  
You can update the live link section above after deployment and continue extending the project with backend services later.
