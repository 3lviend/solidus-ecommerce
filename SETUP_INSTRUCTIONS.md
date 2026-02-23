# Solidus Store Setup Instructions

This guide will help you set up a complete Solidus e-commerce store with both storefront and admin interface, similar to https://demo.solidus.io/

## Prerequisites

- Ruby (3.2.0 or higher)
- Rails 8.0+
- PostgreSQL (or MySQL)
- ImageMagick or libvips (for image processing)

## Step-by-Step Setup

### 0. Clone repo
```bash
git clone git@github.com:3lviend/solidus-ecommerce.git
cd solidus-ecommerce
```

### 1. Install Dependencies

Make sure all gems are installed:

```bash
bundle install
```

### 2. Create Database

```bash
bin/rails db:drop db:create
```

### 3. Install Solidus

Run the Solidus installer(use auto-accept to use defaults):

Note:
- Ignore if any files conflicted
- This command will populate the sample data also from Solidus

```bash
bin/rails g solidus:install --auto-accept
```

Default admin credentials:
- Email: `admin@example.com`
- Password: `test123`

### 4. Run Migrations

```bash
bin/rails db:migrate
```

### 5. Start the Server

```bash
bin/rails s
```

## Access Your Store

- **Storefront**: http://localhost:3000
- **Admin Panel**: http://localhost:3000/admin

## Resources

- [Solidus Documentation](https://guides.solidus.io/)
- [Solidus Starter Frontend](https://github.com/solidusio/solidus_starter_frontend)
- [Solidus Slack Community](http://slack.solidus.io/)
