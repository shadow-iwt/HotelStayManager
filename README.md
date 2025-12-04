# HotelStay Manager

A modern, full-stack hotel management system built with React, Express, and PostgreSQL. This application provides a comprehensive solution for managing hotel stays, bookings, and guest information.

## 🚀 Features

- **Modern UI**: Built with React and shadcn/ui components for a beautiful, responsive interface
- **Type-Safe**: Full TypeScript implementation with Zod validation
- **Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **Authentication**: Secure user authentication system
- **Real-time**: WebSocket support for real-time updates
- **API**: RESTful API built with Express.js

## 🛠️ Tech Stack

### Frontend
- **React 18** - UI library
- **TypeScript** - Type safety
- **Vite** - Build tool and dev server
- **TanStack Query** - Data fetching and caching
- **Wouter** - Lightweight routing
- **shadcn/ui** - UI component library
- **Tailwind CSS** - Styling
- **React Hook Form** - Form management

### Backend
- **Express.js** - Web framework
- **PostgreSQL** - Database
- **Drizzle ORM** - Type-safe ORM
- **Zod** - Schema validation
- **Passport.js** - Authentication middleware
- **WebSocket** - Real-time communication

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v18 or higher)
- **PostgreSQL** (v14 or higher)
- **npm** or **yarn**

## 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/shadow-iwt/HotelStayManager.git
   cd HotelStayManager
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env` file in the root directory:
   ```env
   DATABASE_URL=postgresql://username:password@localhost:5432/hotelstay
   PORT=5000
   NODE_ENV=development
   ```

4. **Set up the database**
   ```bash
   npm run db:push
   ```

## 🚀 Running the Application

### Development Mode

Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

### Production Mode

1. **Build the application**
   ```bash
   npm run build
   ```

2. **Start the production server**
   ```bash
   npm start
   ```

## 📁 Project Structure

```
HotelStayManager/
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/    # React components
│   │   ├── pages/         # Page components
│   │   ├── hooks/         # Custom React hooks
│   │   └── lib/           # Utility functions
│   └── public/            # Static assets
├── server/                # Backend Express application
│   ├── index.ts          # Server entry point
│   ├── routes.ts         # API routes
│   ├── db.ts             # Database configuration
│   └── storage.ts        # Storage utilities
├── shared/               # Shared code between client and server
│   └── schema.ts         # Database schemas and types
└── script/               # Build scripts
```

## 🗄️ Database Schema

The application uses Drizzle ORM with PostgreSQL. Current schema includes:

- **Users**: User authentication and management

## 📝 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm start` - Start production server
- `npm run check` - Type check TypeScript
- `npm run db:push` - Push database schema changes

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License.

## 👤 Author

**shadow-iwt**

- GitHub: [@shadow-iwt](https://github.com/shadow-iwt)

## 🙏 Acknowledgments

- Built with [shadcn/ui](https://ui.shadcn.com/)
- Powered by [Drizzle ORM](https://orm.drizzle.team/)
- Styled with [Tailwind CSS](https://tailwindcss.com/)
