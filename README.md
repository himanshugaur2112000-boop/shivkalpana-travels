Let me prepare everything you need to create a perfect GitHub repository for your Shivkalpana Travel Booking App!
Action: file_editor create /app/README.md --file-text "# 🌏 Shivkalpana Travel Booking App

A complete travel booking platform built with Expo React Native (mobile) and FastAPI (backend). Book tours across India with instant confirmation and support.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![React Native](https://img.shields.io/badge/React%20Native-0.81.5-blue.svg)
![Expo](https://img.shields.io/badge/Expo-54.0-000020.svg)
![FastAPI](https://img.shields.io/badge/FastAPI-Latest-009688.svg)

## ✨ Features

### 📱 Mobile App (Expo React Native)
- 🔐 User authentication (JWT-based)
- 🏖️ Browse 7+ tour packages
- 🔍 Search and filter destinations
- 📅 Book trips with traveler details
- 🎫 Apply discount coupons
- 📞 Direct call & WhatsApp support
- 📊 Booking history management
- 👤 User profile

### 🚀 Backend (FastAPI)
- 20+ RESTful APIs
- JWT authentication
- MongoDB integration
- Admin dashboard
- Coupon management
- Booking system
- User management

### 🎯 Tour Packages
- **Long Trips:** Goa (₹15,999), Kashmir (₹24,999), Rajasthan (₹18,999)
- **Short Trips:** Lucknow (₹350), Ayodhya (₹500), Banaras (₹350), Delhi (₹600)

## 🛠 Tech Stack

**Frontend:**
- Expo 54
- React Native 0.81.5
- React Navigation 7
- React Native Elements
- Axios
- AsyncStorage

**Backend:**
- FastAPI
- Motor (MongoDB async driver)
- JWT authentication
- Passlib (password hashing)
- Pydantic (data validation)

**Database:**
- MongoDB

## 📦 Installation

### Prerequisites
- Node.js 18+
- Yarn
- Python 3.11+
- MongoDB

### Backend Setup

```bash
cd backend

# Install dependencies
pip install -r requirements.txt

# Configure environment
cp .env.example .env
# Edit .env with your settings

# Run server
uvicorn server:app --host 0.0.0.0 --port 8001 --reload
```

### Frontend Setup

```bash
cd frontend

# Install dependencies
yarn install

# Configure environment
# Edit .env with backend URL

# Start Expo
yarn start
```

## 📱 Testing on Mobile

### Using Expo Go

1. Install Expo Go:
   - [iOS App Store](https://apps.apple.com/app/expo-go/id982107779)
   - [Android Play Store](https://play.google.com/store/apps/details?id=host.exp.exponent)

2. Run `yarn start` in frontend directory
3. Scan QR code with Expo Go app

### Building Native Apps

```bash
# Install EAS CLI
npm install -g eas-cli

# Build for production
eas build --platform ios
eas build --platform android
```

## 🔧 Configuration

### Backend Environment Variables

Create `backend/.env`:
```env
MONGO_URL=mongodb://localhost:27017
DB_NAME=shivkalpana_db
JWT_SECRET_KEY=your-super-secret-key-here
RAZORPAY_KEY_ID=your-razorpay-key
RAZORPAY_KEY_SECRET=your-razorpay-secret
```

### Frontend Environment Variables

Create `frontend/.env`:
```env
EXPO_PUBLIC_BACKEND_URL=http://localhost:8001
```

### Customize Support Contacts

Edit `frontend/utils/contact.ts`:
```typescript
const SUPPORT_PHONE = '+919876543210';
const SUPPORT_WHATSAPP = '+919876543210';
```

## 📂 Project Structure

```
shivkalpana-travel-app/
├── frontend/                  # Expo React Native app
│   ├── app/                  # Screens (Expo Router)
│   │   ├── (auth)/          # Login & Register
│   │   ├── (tabs)/          # Bottom tabs
│   │   ├── package/         # Package details
│   │   ├── booking/         # Booking details
│   │   └── checkout.tsx     # Booking form
│   ├── contexts/            # React contexts
│   ├── utils/               # Utility functions
│   └── assets/              # Images & fonts
│
└── backend/                  # FastAPI server
    ├── server.py            # Main API file
    ├── requirements.txt     # Python dependencies
    └── .env                 # Environment variables
```

## 🔌 API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `GET /api/auth/me` - Get current user

### Packages
- `GET /api/packages` - List all packages
- `GET /api/packages/{id}` - Get package details
- `POST /api/packages` - Create package (admin)
- `PUT /api/packages/{id}` - Update package (admin)
- `DELETE /api/packages/{id}` - Delete package (admin)

### Bookings
- `POST /api/bookings` - Create booking
- `GET /api/bookings` - Get user bookings
- `GET /api/bookings/{id}` - Get booking details

### Admin
- `GET /api/admin/dashboard` - Dashboard KPIs
- `GET /api/admin/bookings` - All bookings
- `GET /api/admin/users` - All users
- `PUT /api/admin/bookings/{id}/status` - Update status

### Coupons
- `POST /api/admin/coupons` - Create coupon
- `GET /api/admin/coupons` - List coupons
- `GET /api/coupons/validate/{code}` - Validate coupon

## 🧪 Testing

### Backend Testing

```bash
cd backend
pytest
```

### Frontend Testing

```bash
cd frontend
yarn test
```

## 🎨 Screenshots

[Add screenshots of your app here]

## 📱 Features in Detail

### Booking Flow
1. Browse tour packages
2. Select package and view details
3. Choose travel date
4. Add traveler information
5. Apply coupon code (optional)
6. Confirm booking instantly

### Support System
- **Call Support:** Tap to dial support number
- **WhatsApp Support:** Direct WhatsApp message with pre-filled text
- Available on all key screens

### Package Management
- Detailed itineraries
- Day-wise activities
- Inclusions & exclusions
- Pricing per person
- Duration information

## 🚀 Deployment

### Mobile Apps
```bash
# Build and submit to app stores
eas build --platform all
eas submit --platform all
```

### Backend
Deploy to:
- AWS EC2
- Heroku
- DigitalOcean
- Railway

### Database
- MongoDB Atlas (recommended)
- Local MongoDB
- Docker MongoDB

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- Your Name - [Your GitHub](https://github.com/yourusername)

## 🙏 Acknowledgments

- Built with Expo and React Native
- Backend powered by FastAPI
- MongoDB for data storage
- Emergent AI for development assistance

## 📞 Support

For support, email: support@shivkalpana.com

Or reach out via:
- WhatsApp: +919876543210
- Phone: +919876543210

## 🔮 Future Enhancements

- [ ] Payment gateway integration
- [ ] Push notifications
- [ ] Real-time booking updates
- [ ] Multi-language support
- [ ] Admin web panel
- [ ] Trip reviews & ratings
- [ ] Photo gallery for packages
- [ ] Advanced search filters

---

**Made with ❤️ in India**
"
Observation: Overwrite successful: /app/README.md

Fetching debug logs for expo

==> /var/log/supervisor/expo.err.log <==
Check the Ngrok status page for outages: https://status.ngrok.com/
error Command failed with exit code 1.
CommandError: failed to start tunnel

remote gone away

Check the Ngrok status page for outages: https://status.ngrok.com/
error Command failed with exit code 1.
"shadow*" style props are deprecated. Use "boxShadow".
"shadow*" style props are deprecated. Use "boxShadow".
"shadow*" style props are deprecated. Use "boxShadow".
"shadow*" style props are deprecated. Use "boxShadow".
"shadow*" style props are deprecated. Use "boxShadow".
"shadow*" style props are deprecated. Use "boxShadow".
"shadow*" style props are deprecated. Use "boxShadow".
"shadow*" style props are deprecated. Use "boxShadow".
"shadow*" style props are deprecated. Use "boxShadow".
"shadow*" style props are deprecated. Use "boxShadow".
"shadow*" style props are deprecated. Use "boxShadow".
"shadow*" style props are deprecated. Use "boxShadow".

==> /var/log/supervisor/expo.out.log <==
Web Bundled 880ms node_modules/expo-router/entry.js (1 module)
λ Bundled 23ms node_modules/expo-router/node/render.js (1 module)
Web Bundled 332ms node_modules/expo-router/entry.js (1 module)
λ Bundled 21ms node_modules/expo-router/node/render.js (1 module)
Web node_modules/expo-router/entry.js ░░░░░░░░░░░░░░░░  0.0% (0/1)
Web Bundled 749ms node_modules/expo-router/entry.js (1 module)
λ Bundled 23ms node_modules/expo-router/node/render.js (1 module)
Web Bundled 296ms node_modules/expo-router/entry.js (1 module)
Web Bundled 28ms node_modules/expo-router/entry.js (1 module)
 LOG  [web] Logs will appear in the browser console
Web node_modules/expo-router/entry.js ░░░░░░░░░░░░░░░░  0.0% (0/1)
λ Bundled 32ms node_modules/expo-router/node/render.js (1 module)
Web Bundled 877ms node_modules/expo-router/entry.js (1 module)
Web Bundled 26ms node_modules/expo-router/entry.js (1 module)
 LOG  [web] Logs will appear in the browser console
Web node_modules/expo-router/entry.js ░░░░░░░░░░░░░░░░  0.0% (0/1)
λ Bundled 24ms node_modules/expo-router/node/render.js (1 module)
Web Bundled 817ms node_modules/expo-router/entry.js (1 module)
Web Bundled 26ms node_modules/expo-router/entry.js (1 module)
 LOG  [web] Logs will appear in the browser console


Fetching debug logs for backend

==> /var/log/supervisor/backend.err.log <==
    version = _bcrypt.__about__.__version__
              ^^^^^^^^^^^^^^^^^
AttributeError: module 'bcrypt' has no attribute '__about__'
INFO:     Shutting down
INFO:     Waiting for application shutdown.
INFO:     Application shutdown complete.
INFO:     Finished server process [878]
INFO:     Stopping reloader process [149]
INFO:     Will watch for changes in these directories: ['/app/backend']
INFO:     Uvicorn running on http://0.0.0.0:8001 (Press CTRL+C to quit)
INFO:     Started reloader process [1880] using WatchFiles
INFO:     Started server process [1882]
INFO:     Waiting for application startup.
INFO:     Application startup complete.
2026-03-22 13:07:31,811 - passlib.handlers.bcrypt - WARNING - (trapped) error reading bcrypt version
Traceback (most recent call last):
  File "/root/.venv/lib/python3.11/site-packages/passlib/handlers/bcrypt.py", line 620, in _load_backend_mixin
    version = _bcrypt.__about__.__version__
              ^^^^^^^^^^^^^^^^^
AttributeError: module 'bcrypt' has no attribute '__about__'

==> /var/log/supervisor/backend.out.log <==
INFO:     10.169.2.194:56424 - "POST /api/auth/login HTTP/1.1" 401 Unauthorized
INFO:     10.169.9.5:48382 - "POST /api/auth/login HTTP/1.1" 401 Unauthorized
INFO:     10.169.2.194:56424 - "POST /api/auth/login HTTP/1.1" 401 Unauthorized
INFO:     10.169.2.194:54316 - "POST /api/auth/login HTTP/1.1" 200 OK
INFO:     10.169.2.194:54316 - "GET /api/packages HTTP/1.1" 200 OK
INFO:     10.169.2.194:45832 - "GET /api/bookings HTTP/1.1" 200 OK
INFO:     10.169.2.194:50264 - "GET /api/packages HTTP/1.1" 200 OK
INFO:     10.169.2.194:50264 - "GET /api/packages/69bfaf15723f9cc72174403a HTTP/1.1" 200 OK
INFO:     10.169.2.194:50264 - "GET /api/packages/69bfaf15723f9cc72174403a HTTP/1.1" 200 OK
INFO:     10.169.2.194:33364 - "POST /api/bookings HTTP/1.1" 200 OK
INFO:     10.169.2.194:33364 - "POST /api/bookings HTTP/1.1" 200 OK
INFO:     10.169.2.194:33364 - "POST /api/bookings HTTP/1.1" 200 OK
INFO:     10.169.2.194:33364 - "POST /api/bookings HTTP/1.1" 200 OK
INFO:     10.169.2.194:33364 - "POST /api/bookings HTTP/1.1" 200 OK
INFO:     10.169.2.194:33364 - "POST /api/bookings HTTP/1.1" 200 OK
INFO:     10.169.2.194:33364 - "POST /api/bookings HTTP/1.1" 200 OK
INFO:     10.169.2.194:33364 - "POST /api/bookings HTTP/1.1" 200 OK
INFO:     10.169.2.194:33364 - "POST /api/bookings HTTP/1.1" 200 OK
INFO:     10.169.9.5:47048 - "GET /api/packages HTTP/1.1" 200 OK
INFO:     10.169.2.194:37782 - "GET /api/packages HTTP/1.1" 200 OK


Fetching debug logs for mongodb

tail: cannot open '/var/log/supervisor/mongodb*.log' for reading: No such file or directory
