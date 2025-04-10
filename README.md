# ChronoChic - Où l'Élégance Rencontre le Temps


## Overview

ChronoChic is a modern e-commerce platform for fashion retail, built with React (frontend) and Express/MongoDB (backend). The application allows users to browse products, add them to favorites, manage their account, and includes an admin interface for product management.

## Features

- **Product Browsing**: View and search through the collection of fashion items
- **Product Filtering**: Filter products by name and other attributes
- **User Authentication**: Secure login system for customers
- **Favorites System**: Save preferred products to a favorites list
- **Admin Dashboard**: Add, edit, and delete products
- **Responsive Design**: Optimized for both desktop and mobile devices

## Project Structure

The project is organized into two main components:

### Frontend (React/Vite)

```
project/
├── src/
│   ├── apis/           # API integration and fetch functions
│   ├── assets/         # Images, fonts, and global styles
│   ├── components/     # Reusable UI components
│   ├── contexts/       # React context providers
│   ├── data/           # Mock data and constants
│   ├── hooks/          # Custom React hooks
│   ├── pages/          # Page components
│   ├── reducers/       # State management
│   ├── App.jsx         # Main application component
│   ├── main.jsx        # Application entry point
│   └── router.jsx      # Routing configuration
└── ...
```

### Backend (Express/MongoDB)

```
project-backend/
├── controllers/        # Request handlers
├── database/           # Database connection and models
├── queries/            # Database query functions
├── routes/             # API route definitions
├── server.js           # Server entry point
└── ...
```

## Technology Stack

### Frontend
- **React 18**: UI library
- **Vite**: Build tool and development server
- **React Router DOM**: Client-side routing
- **React Hook Form**: Form validation and management
- **Yup**: Schema validation
- **SASS**: CSS preprocessor
- **HTML React Parser**: HTML parsing for rich text content

### Backend
- **Express**: Web server framework
- **MongoDB**: NoSQL database
- **Mongoose**: ODM (Object Data Modeling) for MongoDB
- **Nodemon**: Development server with hot reload
- **CORS**: Cross-Origin Resource Sharing middleware
- **Morgan**: HTTP request logger middleware

## Getting Started

### Prerequisites
- Node.js (v14.x or higher)
- MongoDB (local installation or MongoDB Atlas account)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/chronochic.git
   cd chronochic
   ```

2. Set up the backend:
   ```bash
   cd project-backend
   npm install
   ```

3. Set up the frontend:
   ```bash
   cd ../project
   npm install
   ```

4. Configure the MongoDB connection:
   - Edit `project-backend/database/index.js` to update the MongoDB connection URL if needed

### Running the Application

1. Start the backend server:
   ```bash
   cd project-backend
   npm start
   ```
   The backend will run on http://localhost:5000

2. Start the frontend development server:
   ```bash
   cd ../project
   npm run dev
   ```
   The frontend will run on http://localhost:5173

## API Endpoints

The backend provides the following RESTful API endpoints:

### Products
- `GET /produits`: Get all products
- `GET /produits/:produitId`: Get a specific product
- `POST /produits`: Create a new product
- `PATCH /produits/:produitId`: Update a product
- `DELETE /produits/:produitId`: Delete a product

## Database Schema

### Product Model
```javascript
{
  name: String,      // Product name
  image: String,     // URL to product image
  price: Number,     // Product price
  brand: String      // Product brand
}
```

## Admin Features

1. **Add Products**: Create new product listings with details and images
2. **Edit Products**: Modify existing product information
3. **Delete Products**: Remove products from the catalog

## User Features

1. **Browse Products**: View the product catalog
2. **Search Functionality**: Filter products by name or other attributes
3. **Add to Favorites**: Save preferred products to a favorites list
4. **User Authentication**: Log in to access personalized features

## Development

### Building for Production

To build the frontend for production:
```bash
cd project
npm run build
```

This will generate optimized production files in the `dist` directory.

### Linting

To run the linter:
```bash
cd project
npm run lint
```

## Security

The application implements basic authentication for users with email and password. For production use, additional security measures should be implemented, such as:

- HTTPS
- JWT or session-based authentication
- Input sanitization
- Rate limiting
- Helmet for secure HTTP headers

## Future Enhancements

- Shopping cart functionality
- Payment gateway integration
- User profile management
- Product reviews and ratings
- Advanced search and filtering options
- Inventory management
- Order processing and tracking

## Contributors

- [KOCEILA DJABALLAH](https://github.com/ITNKOC)

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---

© 2024 ChronoChic by ITNKOC. All rights reserved.
