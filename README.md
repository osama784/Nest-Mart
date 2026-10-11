# Nest-Mart

Multi-vendor e-commerce platform built with Django and Django REST Framework — product catalog across vendors and categories, shopping cart, order history, and an admin dashboard for managing products, orders, and users. Session-based authentication for customers and administrators; storefront in Django templates with Tailwind CSS and Alpine.js.

> [!NOTE]
> No live demo — run the app locally using the steps below.

## Features

- **Product catalog** — browse products across vendors and categories.
- **Shopping cart** — add, update, and remove items, and apply coupons.
- **Order history** — view past orders and their delivery/payment status from the dashboard.
- **Admin dashboard** — Django admin for managing products, orders, and users.
- **Session-based authentication** — for customers and administrators.

## Tech Stack

- **Backend:** Python, Django, Django REST Framework
- **Frontend:** Django templates, Tailwind CSS, Alpine.js
- **Database:** configured through `DATABASE_URL` (PostgreSQL or SQLite)
- **Media:** Cloudinary (product and vendor images)

## Getting Started

Requires Python 3. Node.js/npm are only needed if you want to rebuild the frontend assets.

1. Clone the repository:

```
> git clone https://github.com/osama784/Nest-Mart.git
> cd Nest-Mart
```

2. Install the Python dependencies:

```
> python -m venv venv
> source venv/bin/activate   # Windows: venv\Scripts\activate
> pip install -r requirements.txt
```

3. Create a `.env` file in the repository root with your own values for:

- `DJANGO_SECRET_KEY`
- `DATABASE_URL` (e.g. a PostgreSQL connection string, or `sqlite:///db.sqlite3`)
- `CLOUDINARY_CLOUD_NAME`, `CLOUDINARY_PUBLIC_API_KEY`, `CLOUDINARY_SECRET_API_KEY` (image storage)

4. Run the app:

```
> cd Ecommerce
> python manage.py migrate
> python manage.py runserver
```

Optional — rebuild the frontend assets (the built CSS and JS are already committed):

```
> npm install
> npm run dev          # Tailwind CSS in watch mode
> npm run build:alpine # bundle Alpine.js helpers
```

## Contact

- Email: osamadoage8@gmail.com
- Portfolio: https://osamadoage.vercel.app/
