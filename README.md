# Nathaniel Bubune's Portfolio Backend

A full-stack portfolio website with a Node.js/Express backend and integrated frontend.

## Features

- **Portfolio Website**: Complete portfolio with multiple pages (Home, About, Skills, Services, Blogs, Contact)
- **Contact Form**: Functional contact form that sends emails via Gmail SMTP
- **Security**: Rate limiting, CORS, and security headers
- **Responsive Design**: Modern, responsive UI with animations

## Setup Instructions

### 1. Install Dependencies
```bash
npm install
```

### 2. Environment Configuration
Create a `.env` file in the root directory with the following variables:

```env
# Email Configuration
EMAIL_USER=your.email@gmail.com
EMAIL_PASS=your_app_password_here

# Server Configuration
PORT=5000
```

**Important**: For Gmail, you need to use an "App Password" instead of your regular password:
1. Enable 2-factor authentication on your Google account
2. Go to Google Account settings → Security → App passwords
3. Generate an app password for "Mail"
4. Use that password in the `EMAIL_PASS` variable

### 3. Start the Server
```bash
npm start
```

The server will start on `http://localhost:5000`

## Project Structure

```
portfolio-backend/
├── server.js                 # Main server file
├── index.html               # Home page
├── about.html               # About page
├── skills.html              # Skills page
├── services.html            # Services page
├── blogs.html               # Blogs page
├── contact.html             # Contact page
├── style.css                # Main stylesheet
├── controllers/
│   └── contactController.js # Contact form handler
├── routes/
│   └── contact.js           # Contact API routes
└── package.json             # Dependencies
```

## API Endpoints

- `POST /api/contact` - Handle contact form submissions
- `GET /` - Serve home page
- `GET /about` - Serve about page
- `GET /skills` - Serve skills page
- `GET /services` - Serve services page
- `GET /blogs` - Serve blogs page
- `GET /contact` - Serve contact page

## Technologies Used

- **Backend**: Node.js, Express.js
- **Email**: Nodemailer with Gmail SMTP
- **Security**: Helmet, CORS, Rate Limiting
- **Frontend**: HTML5, CSS3, JavaScript
- **Animations**: AOS (Animate On Scroll)

## Contact Form

The contact form is fully functional and will:
1. Validate required fields
2. Send emails to your configured Gmail address
3. Show success/error messages to users
4. Prevent spam with rate limiting

## Development

To run in development mode with auto-restart:
```bash
npm install -g nodemon
nodemon server.js
``` 