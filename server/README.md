# EventDuniya Server

Backend API server for the EventDuniya platform.

## Setup Instructions

1. Install dependencies:
   ```
   npm install
   ```

2. Create a `.env` file in the root directory with the following variables:
   ```
   MONGO_URI=your_mongodb_connection_string
   ACCESS_TOKEN_LIFE_SECOND=900
   REFRESH_TOKEN_LIFE_SECOND=604800
   ACCESS_TOKEN_SECRET=your_access_token_secret
   REFRESH_TOKEN_SECRET=your_refresh_token_secret
   NODE_ENV=development
   GOOGLE_AUTH=your_google_auth_client_id
   SECRET_COOKIE=your_cookie_secret
   FRONTEND_URL=http://localhost:5173
   RAZORPAY_KEY_ID=your_razorpay_key_id
   RAZORPAY_KEY_SECRET=your_razorpay_key_secret
   ```

3. Build the project:
   ```
   npm run build
   ```

4. Start the server:
   ```
   npm start
   ```

5. For development with hot reloading:
   ```
   npm run dev
   ```

## API Routes

- `/api/payments` - Razorpay payment integration
- `/api/auth` - Authentication routes
- `/api/events` - Event management
- `/api/user` - User operations
- `/api/artist` - Artist profiles
- `/api/bookticket` - Event ticket booking
- `/api/review` - Artist reviews
- `/api/image` - Image uploads
- `/api/contact` - Contact form
- `/api/savedartist` - Favorite artist management

## Technology Stack

- Node.js
- Express
- MongoDB with Mongoose
- TypeScript
- Razorpay Payment Gateway
- AWS S3 for file storage
