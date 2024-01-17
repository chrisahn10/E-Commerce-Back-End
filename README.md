# E-Commerce-Back-End

## Description
This project is a backend system for an e-commerce site. It uses Node.js, Express.js, and Sequelize to manage a MySQL database that stores data about products, categories, and tags.

## Installation

### Prerequisites
- Node.js
- MySQL

### Steps
1. Clone the repository to your local machine.
2. Run `npm install` to install dependencies.
3. Configure your MySQL credentials in a `.env` file.
4. Run `npm run seed` to seed the database.
5. Start the server with `npm start`.

## Usage
This system allows you to manage an e-commerce database with the following models:
- **Product**: Represents items for sale.
- **Category**: Represents categories under which products are organized.
- **Tag**: Represents tags that can be associated with products.
- **ProductTag**: Represents associations between products and tags.

### API Endpoints
- `/api/products`: CRUD operations for products.
- `/api/categories`: CRUD operations for categories.
- `/api/tags`: CRUD operations for tags.

## Models

### Product
- Fields: id, product_name, price, stock, category_id
- Relationships: Belongs to Category, has many ProductTag

### Category
- Fields: id, category_name
- Relationships: Has many Product

### Tag
- Fields: id, tag_name
- Relationships: Has many ProductTag

### ProductTag
- Fields: id, product_id, tag_id
- Relationships: Belongs to Product, belongs to Tag

## Scripts
- `npm start`: Starts the server.
- `npm run seed`: Seeds the database with initial data.

## Contributing
Contributions are welcome. Please open an issue or a pull request to suggest changes or additions.

## License
[MIT](LICENSE)

## Questions
For any questions, please contact [Your Name](your-email@example.com).
