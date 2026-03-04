# 🍽️ RestaurantGraphura

A modern, full-stack restaurant management system built for Graphura India Pvt Ltd. This comprehensive solution streamlines restaurant operations including menu management, order processing, reservations, kitchen operations, and analytics.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Node](https://img.shields.io/badge/node-%3E%3D18.0.0-brightgreen)
![React](https://img.shields.io/badge/react-19.2.0-blue)

## 🚀 Features

### Customer Features
- 🔐 **User Authentication** - Secure JWT-based login and registration
- 📱 **Interactive Menu** - Browse categorized menu items with images and prices
- 🛒 **Cart Management** - Add, remove, and modify orders before checkout
- 💳 **Payment Integration** - Razorpay payment gateway for secure transactions
- 📅 **Table Reservations** - Book tables with real-time availability
- 💬 **Feedback System** - Submit reviews and ratings for dining experience
- 📧 **Email Notifications** - Order confirmations and updates via email

### Admin Features
- 📊 **Analytics Dashboard** - Comprehensive insights with interactive charts (Recharts)
- 🍕 **Menu Management** - Add, edit, delete menu items and categories
- 📦 **Order Tracking** - Monitor and manage customer orders in real-time
- 👨‍🍳 **Kitchen Dashboard** - Kitchen order management and status updates
- 📈 **Sales Reports** - Revenue tracking and performance metrics
- 👥 **User Management** - Admin access control and user roles

### Technical Features
- ⚡ **Fast Performance** - Vite for lightning-fast frontend builds
- 🎨 **Modern UI/UX** - Framer Motion animations and responsive design
- 🔒 **Security** - Rate limiting, input validation, and secure authentication
- 📱 **Responsive Design** - Works seamlessly on desktop, tablet, and mobile
- 🎯 **RESTful API** - Well-structured backend with Express.js

## 🛠️ Tech Stack

### Frontend
- **React 19.2** - Modern UI library with latest features
- **Vite** - Next-generation frontend tooling
- **React Router DOM** - Client-side routing
- **Axios** - HTTP client for API requests
- **Framer Motion** - Animation library
- **Recharts** - Data visualization
- **Lucide React** - Icon library
- **React Icons** - Additional icon sets

### Backend
- **Node.js** - JavaScript runtime
- **Express.js 5** - Web application framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB ODM
- **JWT** - JSON Web Tokens for authentication
- **Bcrypt** - Password hashing
- **Razorpay** - Payment gateway integration
- **Nodemailer** - Email service
- **Express Validator** - Input validation
- **Express Rate Limit** - API rate limiting
- **Cookie Parser** - Cookie handling
- **CORS** - Cross-origin resource sharing

## 📦 Project Structure

```
RestaurantGraphura/
├── restaurant/
│   └── restaurant system(final)/
│       ├── backend/           # Backend API server
│       │   ├── src/
│       │   │   ├── controllers/
│       │   │   ├── models/
│       │   │   ├── routes/
│       │   │   ├── middleware/
│       │   │   └── utils/
│       │   ├── server.js      # Entry point
│       │   └── package.json
│       │
│       └── DineFlow/          # Frontend React app
│           ├── src/
│           │   ├── components/
│           │   ├── pages/
│           │   ├── context/
│           │   ├── routes/
│           │   ├── assets/
│           │   └── config/
│           ├── public/
│           └── package.json
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- MongoDB (local or Atlas)
- npm or yarn package manager
- Razorpay account (for payment integration)

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/mukeshk78254/RestaurantGraphura.git
cd RestaurantGraphura
```

2. **Backend Setup**
```bash
cd restaurant/restaurant\ system\(final\)/backend
npm install
```

Create `.env` file in the backend directory:
```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=587
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_email_password
NODE_ENV=development
```

3. **Frontend Setup**
```bash
cd ../DineFlow
npm install
```

Create `.env` file in the DineFlow directory:
```env
VITE_API_URL=http://localhost:5000/api
VITE_RAZORPAY_KEY_ID=your_razorpay_key_id
```

### Running the Application

**Start Backend Server:**
```bash
cd backend
npm run dev          # Development mode with nodemon
# or
npm start           # Production mode
```
Backend runs on: `http://localhost:5000`

**Start Frontend:**
```bash
cd DineFlow
npm run dev         # Development mode
# or
npm run build       # Build for production
npm run preview     # Preview production build
```
Frontend runs on: `http://localhost:5173`

## 📝 API Documentation

### Authentication Endpoints
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout
- `GET /api/auth/profile` - Get user profile

### Menu Endpoints
- `GET /api/menu` - Get all menu items
- `GET /api/menu/:id` - Get menu item by ID
- `POST /api/menu` - Create menu item (Admin)
- `PUT /api/menu/:id` - Update menu item (Admin)
- `DELETE /api/menu/:id` - Delete menu item (Admin)

### Order Endpoints
- `GET /api/orders` - Get all orders
- `POST /api/orders` - Create new order
- `GET /api/orders/:id` - Get order details
- `PUT /api/orders/:id` - Update order status

### Additional Endpoints
- Category Management
- Reservation System
- Payment Processing
- Kitchen Operations
- Analytics & Reports
- Catering Services
- Contact & Feedback

## 🔒 Security Features

- JWT-based authentication with HTTP-only cookies
- Password hashing using bcrypt
- Input validation and sanitization
- Rate limiting to prevent abuse
- CORS configuration for secure cross-origin requests
- Environment variable protection
- Secure payment processing with Razorpay

## 🎨 UI/UX Features

- Clean and modern interface
- Smooth animations with Framer Motion
- Responsive design for all devices
- Interactive data visualizations
- Real-time order status updates
- Toast notifications for user feedback
- Loading states and error handling

## 🧪 Testing

```bash
npm test
```

## 📱 Deployment

### Backend Deployment (Render)
The backend includes a `render.yaml` configuration for easy deployment on Render.

### Frontend Deployment (Vercel)
The frontend includes a `vercel.json` configuration for Vercel deployment.

## 🤝 Contributing

This project was developed for Graphura India Pvt Ltd. For internal contributions:

1. Create a feature branch
2. Make your changes
3. Submit a pull request
4. Wait for code review

## 📄 License

This project is proprietary and confidential. 
© 2026 Graphura India Pvt Ltd. All rights reserved.

## 👥 Team

Developed with ❤️ by the Graphura India Pvt Ltd team

## 📞 Support

For support and queries:
- Email: support@graphura.com
- Website: www.graphura.com

## 🙏 Acknowledgments

- Graphura India Pvt Ltd for project opportunity
- Open-source community for amazing tools and libraries
- React and Node.js communities

---

**Note:** This is an internal project for Graphura India Pvt Ltd. Sensitive information including database credentials, API keys, and configuration details are protected and not included in version control.
