# Peer-Mart - College Marketplace

A college-based marketplace where students can buy, sell, and trade items using a coin system and college-specific listings.

## Features

- College-based user system with filtered listings  
- Coin-based economy for buying and trading  
- Trade system supporting items and coin negotiation  
- Real-time chat between users  
- Product listing and management system  
- Search and filtering functionality  
- Responsive design for desktop and mobile  

## Tech Stack

- Frontend: React 18, Tailwind CSS, Framer Motion, Axios  
- Backend: Node.js, Express.js  
- Database: MongoDB, Mongoose  
- Authentication: JWT, bcrypt  
- File Uploads: Multer  
- Real-time Communication: Socket.IO  

## Quick Start

### 1. Clone and Setup

```bash
git clone <your-repo-url>
cd college-marketplace
```

### 2. Install Dependencies

```bash
npm install

cd server
npm install
cd ..
```

### 3. Setup Database

Ensure MongoDB is running at:

```
mongodb://localhost:27017
```

The database `cdsc` will be created automatically.

### 4. Seed Initial Data

```bash
cd server
node seedData.js
cd ..
```

### 5. Environment Variables (Optional)

Create a `server/.env` file:

```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/cdsc
JWT_SECRET=your-secret-key
```

## Running the Application

### Option 1: Windows

```bash
start.bat
```

### Option 2: Manual

Backend:

```bash
cd server
npm run dev
```

Frontend:

```bash
npm run dev
```

## Access

- Frontend: http://localhost:5173  
- Backend API: http://localhost:5000  

## How It Works

### Coin System
- Initial balance: 100 coins  
- Listing a product: +50 coins  
- Completing a trade: +100 coins for both users  

### Trading Flow
1. Select a product marked for trade  
2. Initiate trade request  
3. Add items and/or coins  
4. Submit proposal  
5. Await response  

### Product Management
- Upload up to 5 images per product  
- Add description, category, and condition  
- Edit or delete listings  

## API Endpoints

### Authentication
- POST `/api/register`  
- POST `/api/signin`  

### Products
- GET `/api/products`  
- POST `/api/products`  

### Trades
- GET `/api/trades`  
- POST `/api/trades`  
- PUT `/api/trades/:id`  

### Purchase
- POST `/api/purchase`  

## Project Structure

```
college-marketplace/
├── src/
├── server/
├── package.json
├── start.bat
└── README.md
```

## Additional Features

- Cross-college trading support  
- Multi-item trade proposals  
- Real-time notifications  
- Secure authentication system  

## License

MIT License  

## Support

For issues or questions, open an issue in the repository.
