# Portfolio Website Deployment Guide

## Deploy to Netlify (Recommended - Free)

### Option 1: Deploy via Netlify UI (Easiest)

1. **Prepare your files:**
   - Make sure all your HTML, CSS, and image files are in the project directory
   - The `netlify.toml` file is already configured

2. **Go to Netlify:**
   - Visit [netlify.com](https://netlify.com)
   - Sign up/Login with your GitHub account

3. **Deploy:**
   - Click "New site from Git"
   - Choose your repository
   - Set build command: (leave empty)
   - Set publish directory: `.` (current directory)
   - Click "Deploy site"

### Option 2: Deploy via Netlify CLI

1. **Install Netlify CLI:**
   ```bash
   npm install -g netlify-cli
   ```

2. **Login to Netlify:**
   ```bash
   netlify login
   ```

3. **Deploy:**
   ```bash
   netlify deploy --prod
   ```

### Option 3: Drag & Drop (Quick Test)

1. **Zip your files:**
   - Select all files except `node_modules/`, `package-lock.json`, and `.git/`
   - Create a ZIP file

2. **Deploy:**
   - Go to [netlify.com](https://netlify.com)
   - Drag and drop your ZIP file to the deploy area

## Alternative Deployment Options

### GitHub Pages
- Push to GitHub repository
- Enable GitHub Pages in repository settings
- Set source to main branch

### Vercel
- Visit [vercel.com](https://vercel.com)
- Import your GitHub repository
- Automatic deployment

### Firebase Hosting
- Install Firebase CLI: `npm install -g firebase-tools`
- Initialize: `firebase init hosting`
- Deploy: `firebase deploy`

## Post-Deployment

1. **Custom Domain (Optional):**
   - In Netlify dashboard, go to Domain settings
   - Add your custom domain

2. **Environment Variables:**
   - If you add backend features later, set environment variables in Netlify dashboard

3. **Form Handling:**
   - Your contact form is already configured with Formspree
   - No additional setup needed

## File Structure for Deployment

```
portfolio-backend/
├── index.html          # Homepage
├── about.html          # About page
├── skills.html         # Skills page
├── services.html       # Services page
├── blogs.html          # Blog page
├── contact.html        # Contact page
├── style.css           # Main stylesheet
├── myself.jpeg         # Profile picture
├── netlify.toml        # Netlify configuration
├── .gitignore          # Git ignore file
└── README.md           # Project documentation
```

## Notes

- Your contact form uses Formspree and will work immediately
- All animations and styling will work on the deployed site
- The site is fully responsive and mobile-friendly
- No backend server needed for static deployment 