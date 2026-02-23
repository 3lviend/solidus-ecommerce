# Solidus Store

A complete e-commerce store built with [Solidus](https://solidus.io/), an open-source e-commerce platform for Ruby on Rails. This application provides both a storefront for customers and an admin panel for managing products, orders, and inventory.

## Features

- 🛒 **Full-featured storefront** - Complete shopping experience with product browsing, cart, and checkout
- 👨‍💼 **Admin panel** - Comprehensive admin interface for managing products, orders, customers, and more
- 💳 **Payment integration** - PayPal Commerce Platform integration included
- 🎨 **Modern UI** - Built with Tailwind CSS and View Components
- 📦 **Sample data** - Pre-configured with sample products and categories

## Getting Started

For detailed setup instructions, see [SETUP_INSTRUCTIONS.md](./SETUP_INSTRUCTIONS.md).

## Configuration

Database configuration is in `config/database.yml`. Update it with your database credentials if needed.

## Testing

Run the test suite:

```bash
# Run all tests
bundle exec rspec

# Run specific test file
bundle exec rspec spec/path/to/test_spec.rb
```

## Services

This application uses:

- **Solid Cache** - Database-backed caching
- **Solid Queue** - Database-backed job queue
- **Solid Cable** - Database-backed Action Cable adapter
- **Puma** - Web server

## Deployment

This application is configured for deployment with Kamal. See `config/deploy.yml` for deployment configuration.

## Documentation

For more detailed setup instructions, see:
- [SETUP_INSTRUCTIONS.md](./SETUP_INSTRUCTIONS.md) - Detailed step-by-step setup guide

## License

This project uses Solidus, which is licensed under the BSD-3-Clause license.
