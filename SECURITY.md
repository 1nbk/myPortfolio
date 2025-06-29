# Security Guidelines for Portfolio Website

## 🔒 Credential Protection

### What's Protected
- **Email Address**: gbknathaniel@gmail.com
- **Phone Number**: +233 536034346
- **Location**: Kumasi KNUST
- **Formspree Endpoint**: https://formspree.io/f/xqabwooy

### Security Measures Implemented

#### 1. Git Protection
- ✅ `.gitignore` updated to exclude sensitive files
- ✅ Environment files (`.env`, `.env.local`, etc.) are ignored
- ✅ Template files created for public sharing
- ✅ No credentials in public repository

#### 2. File Protection
- ✅ Sensitive files excluded from version control
- ✅ Template files for public display
- ✅ Backup files ignored

#### 3. Best Practices
- ✅ Never commit `.env` files
- ✅ Use environment variables for sensitive data
- ✅ Template files for public repositories
- ✅ Regular security audits

## 🛡️ Security Checklist

### Before Committing
- [ ] No real email addresses in code
- [ ] No real phone numbers in code
- [ ] No API keys or endpoints exposed
- [ ] No personal information in public files

### For Deployment
- [ ] Use environment variables
- [ ] Secure form endpoints
- [ ] HTTPS enabled
- [ ] Regular security updates

## 📁 File Structure

```
portfolio-backend/
├── contact.html          # Live site (contains real credentials)
├── contact.template.html # Template (no real credentials)
├── .env                  # Environment variables (ignored by Git)
├── .gitignore           # Git ignore rules
├── SECURITY.md          # This security guide
└── ...other files
```

## 🚨 Important Notes

1. **Never share the `.env` file**
2. **Use template files for public repositories**
3. **Regularly update dependencies**
4. **Monitor for security vulnerabilities**
5. **Use HTTPS in production**

## 🔧 Environment Setup

Create a `.env` file (not committed to Git):
```bash
CONTACT_EMAIL=your-email@example.com
CONTACT_PHONE=your-phone-number
CONTACT_LOCATION=your-location
FORMSPREE_ENDPOINT=your-formspree-endpoint
```

## 📞 Contact for Security Issues

If you find any security vulnerabilities, please contact:
- Email: gbknathaniel@gmail.com
- Phone: +233 536034346

---

**Last Updated**: June 2025
**Security Level**: High 