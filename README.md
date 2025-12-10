# URL Shortener

A full-stack URL shortening application that allows users to convert long URLs into short, shareable links.

## 🚀 Features

- **URL Shortening**: Convert long URLs into short, easy-to-share links
- **Custom Short URLs**: Generate unique short codes for each URL
- **URL Validation**: Validates URLs before shortening
- **Modern UI**: Clean and responsive interface built with React and Tailwind CSS
- **RESTful API**: Express.js backend with MongoDB database
- **Real-time Updates**: Dynamic URL list management

## 🛠️ Technologies & Tools

### Frontend
- **React** (v18.2.0) - UI library
- **Tailwind CSS** (v3.3.2) - Utility-first CSS framework
- **React Icons** (v4.10.1) - Icon library
- **React Spinners** (v0.13.8) - Loading indicators

### Backend
- **Node.js** - Runtime environment
- **Express.js** (v4.18.2) - Web framework
- **MongoDB** - NoSQL database
- **Mongoose** (v7.3.1) - MongoDB ODM

### Additional Tools
- **nanoid** (v3.0.0) - Unique ID generator
- **CORS** (v2.8.5) - Cross-Origin Resource Sharing
- **dotenv** (v16.3.1) - Environment variable management
- **Nodemon** (v3.0.2) - Development auto-reload

## 📋 Prerequisites

Before running this application, make sure you have the following installed:
- Node.js (v14 or higher)
- npm or yarn
- MongoDB (local installation or MongoDB Atlas account)

## 🔧 Installation & Setup

### Quick Start (Using provided scripts)

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd URL-Shortener-main
   ```

2. **Install dependencies**
   ```bash
   ./install.sh
   ```

3. **Configure environment variables**
   
   Create a `.env` file in the `server` directory:
   ```env
   MONGODB_URI=your_mongodb_connection_string
   PORT=5000
   ```
   
   Create a `.env` file in the `client` directory:
   ```env
   REACT_APP_API_URL=http://localhost:5000
   ```

4. **Run the application**
   ```bash
   ./run.sh
   ```

### Manual Setup

#### Backend Setup
```bash
cd server
npm install
npm run dev
```

#### Frontend Setup
```bash
cd client
npm install
npm start
```

## 🏗️ Project Structure

```
URL-Shortener-main/
├── client/                 # React frontend
│   ├── public/
│   ├── src/
│   │   ├── components/    # React components
│   │   │   ├── CallToAction.jsx
│   │   │   ├── Header.jsx
│   │   │   ├── Hero.jsx
│   │   │   ├── Main.jsx
│   │   │   ├── Shortener.jsx
│   │   │   └── UrlList.jsx
│   │   ├── images/        # Image assets
│   │   ├── App.js
│   │   └── index.js
│   └── package.json
│
└── server/                # Express backend
    ├── controllers/       # Route controllers
    │   └── url.js
    ├── models/           # Database models
    │   └── Url.js
    ├── routes/           # API routes
    │   └── index.js
    ├── utils/            # Utility functions
    │   ├── generateUniqueId.js
    │   └── validateUrl.js
    ├── server.js         # Entry point
    └── package.json
```

## 🌐 API Endpoints

- `POST /api/shorten` - Create a shortened URL
- `GET /api/:shortId` - Redirect to original URL
- `GET /api/urls` - Get all shortened URLs

## 💻 Usage

1. Open your browser and navigate to `http://localhost:3000`
2. Enter a long URL in the input field
3. Click the "Shorten" button
4. Copy and share your shortened URL
5. View all your shortened URLs in the list below

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

