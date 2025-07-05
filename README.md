# GrowthPro - Mini Local Business Dashboard

A full-stack JavaScript application for local business analytics and SEO optimization.

## 🔧 Technology Stack

**Frontend:** React (Vite) + Tailwind CSS - JavaScript Only (.js, .jsx)  
**Backend:** Node.js + Express - JavaScript Only (.js)  
**CORS:** Enabled for cross-origin requests  
**Database:** None (simulated data)

## 📦 Project Structure

```
GrowthPro/
├── growthpro-frontend/     # React frontend (JavaScript only)
│   ├── src/
│   │   ├── components/     # React components (.jsx)
│   │   ├── pages/         # Page components (.jsx)
│   │   ├── lib/           # Utilities and API (.js)
│   │   └── main.jsx       # Application entry point
│   ├── index.html
│   ├── package.json
│   └── README.md
└── growthpro-backend/      # Express backend (JavaScript only)
    ├── server.js          # Main server file
    ├── package.json
    └── README.md
```

## 🎯 Application Features

### Frontend Features
- ✅ **Business Form** with name and location inputs
- ✅ **Form Validation** with error handling
- ✅ **Loading Spinners** during API calls
- ✅ **Responsive Design** with Tailwind CSS
- ✅ **Business Results Display** with rating stars and review counts
- ✅ **AI-Generated SEO Headlines** with regeneration feature
- ✅ **Mobile-Friendly** responsive layout

### Backend Features
- ✅ **POST /business-data** - Submit business data and get analytics
- ✅ **GET /regenerate-headline** - Generate new SEO headlines
- ✅ **CORS Enabled** for frontend communication
- ✅ **Input Validation** and error handling
- ✅ **Simulated Data** - no database required
- ✅ **Realistic Business Metrics** (4.0-5.0 ratings, 50-500 reviews)

## 🚀 Quick Start

### 1. Frontend Setup (React + Vite)

```bash
# Install frontend dependencies
npm install

# Start development server
npm run dev
```

The frontend will run on **http://localhost:8080**

### 2. Backend Setup (Node.js + Express)

See [BACKEND_CODE.md](./BACKEND_CODE.md) for complete backend implementation.

```bash
# Create backend folder
mkdir growthpro-backend && cd growthpro-backend

# Initialize project
npm init -y

# Install dependencies
npm install express cors
npm install -D nodemon

# Copy server.js from BACKEND_CODE.md
# Start backend server
npm run dev
```

The backend will run on **http://localhost:3001**

## 🔗 API Endpoints

### POST /business-data
Submit business information to get analytics.

**Request:**
```json
{
  "name": "Joe's Pizza",
  "location": "New York, NY"
}
```

**Response:**
```json
{
  "name": "Joe's Pizza",
  "location": "New York, NY",
  "rating": 4.7,
  "reviews": 234,
  "headline": "Top-Rated Joe's Pizza in New York, NY - Trusted by 234+ Happy Customers"
}
```

### GET /regenerate-headline
Generate new SEO headline for existing business.

**Request:**
```
GET /regenerate-headline?name=Joe's Pizza&location=New York, NY
```

**Response:**
```json
{
  "headline": "Best Joe's Pizza Experience in New York, NY - 156 Five-Star Reviews"
}
```

## 💻 Development

### Frontend Scripts
```bash
npm run dev          # Start development server
npm run build        # Build for production
npm run preview      # Preview production build
npm run lint         # Run ESLint
```

### Backend Scripts
```bash
npm start            # Start production server
npm run dev          # Start with nodemon (auto-reload)
```

## 🎨 Design System

The application uses a custom design system with:
- **Semantic Color Tokens** (primary, success, warning, info)
- **Responsive Tailwind Classes**
- **Gradient Backgrounds** and modern UI
- **Dark/Light Mode Support**
- **Glass-morphism Effects** on cards

## ⚠️ Important Notes

- **JavaScript Only:** This project uses 0% TypeScript - all files are .js/.jsx
- **No Database:** All data is simulated for demonstration
- **CORS Enabled:** Backend configured for frontend communication
- **Mobile Responsive:** Works on all device sizes
- **Production Ready:** Includes error handling and validation

## 🔄 Connecting Frontend to Backend

1. **Start both servers** (frontend on 8080, backend on 3001)
2. **Update API calls** in `src/lib/api.js`:
   - Replace `mockAPI` usage with actual fetch calls to `http://localhost:3001`
   - Backend endpoints are ready and CORS-enabled

## 📱 Screenshots

The application features a modern, responsive design with:
- Clean business form with validation
- Beautiful results cards with ratings and reviews
- AI-generated SEO headlines with regeneration
- Loading states and smooth transitions
- Mobile-optimized layout

## 🤝 Contributing

This is a demonstration project showcasing full-stack JavaScript development with React and Express.

## 📄 License

MIT License - Feel free to use this code for learning and development.

---

**Tech Stack Summary:** React + Vite + Tailwind + Node.js + Express (100% JavaScript)
