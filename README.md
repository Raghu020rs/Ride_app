# 🚗 Ride App - Uber Clone

A full-stack ride-sharing application built with **MERN Stack** (MongoDB, Express, React, Node.js) featuring real-time location tracking, user and driver authentication, and Socket.io for live updates.

## 📋 Features

### User Features
- 🔐 User authentication (Login/Signup)
- 📍 Location search and autocomplete
- 🚕 Multiple vehicle options (Car, Moto, Auto)
- 💰 Real-time fare calculation
- 🗺️ Live ride tracking with Google Maps
- ⏱️ Real-time driver location updates
- 📱 Responsive mobile-first design

### Captain (Driver) Features
- 🔐 Captain authentication with vehicle details
- 📊 Real-time ride requests
- ✅ Accept/Decline ride requests
- 🚗 Live navigation to pickup and drop locations
- 💵 Ride completion and payment tracking
- 📈 Captain dashboard with earnings

### Technical Features
- 🔄 Real-time communication using Socket.io
- 🗺️ Google Maps API integration
- 🔒 JWT-based authentication
- 🎨 Tailwind CSS for styling
- 📱 Fully responsive design
- 🚀 Fast build with Vite

## 🛠️ Tech Stack

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - Database
- **Mongoose** - ODM
- **Socket.io** - Real-time communication
- **JWT** - Authentication
- **Bcrypt** - Password hashing
- **Axios** - HTTP client for Google Maps API

### Frontend
- **React 18** - UI library
- **Vite** - Build tool
- **React Router DOM** - Routing
- **Tailwind CSS** - Styling
- **Socket.io Client** - Real-time updates
- **GSAP** - Animations
- **Google Maps API** - Maps integration
- **Axios** - API calls

## 📁 Project Structure

```
Ride_app/
├── Backend/
│   ├── controllers/      # Request handlers
│   ├── db/              # Database configuration
│   ├── middlewares/     # Auth & validation
│   ├── models/          # Database schemas
│   ├── routes/          # API routes
│   ├── services/        # Business logic
│   ├── app.js           # Express app setup
│   ├── server.js        # Server entry point
│   └── socket.js        # Socket.io configuration
│
└── frontend/
    ├── src/
    │   ├── components/  # Reusable UI components
    │   ├── pages/       # Page components
    │   ├── context/     # React Context API
    │   └── assets/      # Static assets
    └── public/          # Public files
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- MongoDB (local or Atlas)
- Google Maps API Key

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/Raghu020rs/Ride_app.git
cd Ride_app
```

2. **Setup Backend**
```bash
cd Backend
npm install
```

Create `.env` file in Backend folder:
```env
PORT=4000
DB_CONNECT=mongodb://localhost:27017/uber-app
JWT_SECRET=your-secret-key-here
GOOGLE_MAPS_API=your-google-maps-api-key
FRONTEND_URL=http://localhost:5173
```

3. **Setup Frontend**
```bash
cd frontend
npm install
```

Create `.env` file in frontend folder:
```env
VITE_BASE_URL=http://localhost:4000
VITE_GOOGLE_MAPS_API_KEY=your-google-maps-api-key
```

4. **Run the Application**

Terminal 1 - Backend:
```bash
cd Backend
npm start
```

Terminal 2 - Frontend:
```bash
cd frontend
npm run dev
```

5. **Access the app**
- Frontend: `http://localhost:5173`
- Backend: `http://localhost:4000`

## 🔑 Environment Variables

### Backend (.env)
| Variable | Description |
|----------|-------------|
| `PORT` | Server port (default: 4000) |
| `DB_CONNECT` | MongoDB connection string |
| `JWT_SECRET` | Secret key for JWT tokens |
| `GOOGLE_MAPS_API` | Google Maps API key |
| `FRONTEND_URL` | Frontend URL for CORS |

### Frontend (.env)
| Variable | Description |
|----------|-------------|
| `VITE_BASE_URL` | Backend API URL |
| `VITE_GOOGLE_MAPS_API_KEY` | Google Maps API key |

## 📱 API Endpoints

### User Routes
- `POST /users/register` - Register new user
- `POST /users/login` - User login
- `GET /users/profile` - Get user profile
- `GET /users/logout` - User logout

### Captain Routes
- `POST /captains/register` - Register new captain
- `POST /captains/login` - Captain login
- `GET /captains/profile` - Get captain profile
- `GET /captains/logout` - Captain logout

### Ride Routes
- `POST /rides/create` - Create new ride
- `GET /rides/get-fare` - Calculate ride fare
- `POST /rides/confirm` - Confirm ride
- `GET /rides/start-ride` - Start ride
- `POST /rides/end-ride` - End ride

### Maps Routes
- `GET /maps/get-coordinates` - Get location coordinates
- `GET /maps/get-distance-time` - Calculate distance and time
- `GET /maps/get-suggestions` - Get location suggestions

## 🎨 Screenshots

*(Add your screenshots here)*

## 🚧 Future Enhancements

- [ ] Payment gateway integration
- [ ] Ride history and receipts
- [ ] Driver ratings and reviews
- [ ] In-app chat between user and driver
- [ ] Push notifications
- [ ] Admin dashboard
- [ ] Multi-language support
- [ ] Ride scheduling

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**Raghu**
- GitHub: [@Raghu020rs](https://github.com/Raghu020rs)

## 🙏 Acknowledgments

- Inspired by Uber's ride-sharing platform
- Google Maps API for location services
- Socket.io for real-time features
- React and Node.js communities

---

⭐ **Star this repo if you find it helpful!**

