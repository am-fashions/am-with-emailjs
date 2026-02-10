# 🔐 Production Configuration Reference

## Quick Reference for Deployment

### 📧 Email Configuration
```
Service: Gmail
Email: madasumiteesh@gmail.com
App Password: mnfc xdxe ojpi rtzf
Admin Email: madasumiteesh@gmail.com
```

### 💳 Payment Information
```
UPI ID: 6281534110-2@ybl
Payment Method: UPI (QR Code + Manual Entry)
Transaction ID: 12-digit number required
Screenshot: Required for verification
```

### 📱 Contact Information
```
Email: madasumiteesh@gmail.com
WhatsApp: +91 91009 11697
Location: Anantapur, Andhra Pradesh 515001
Instagram: https://www.instagram.com/am_fashions.official?igsh=MWU5a3F2eXprYW8ybQ==
```

### 🔑 Default Admin Credentials (CHANGE IN PRODUCTION!)
```
Username: admin
Password: admin123
```

### 🗄️ Database Configuration
```
Database Name: ecommerce_admin
Tables: 13 tables including payment_verifications, login_requests
Character Set: utf8mb4
Collation: utf8mb4_unicode_ci
```

### 🌐 Current Local URLs
```
Main Website: http://localhost:3000
Admin Dashboard: http://localhost:3001
Backend API: http://localhost:5000
```

### 📂 Important Directories
```
Main Website Build: am-with-emailjs/build/
Admin Dashboard Build: am-with-emailjs/admin-dashboard/client/dist/
Backend Server: am-with-emailjs/admin-dashboard/server/
Database Scripts: am-with-emailjs/admin-dashboard/database/
Uploads: am-with-emailjs/admin-dashboard/server/uploads/
```

### 🔄 Build Commands
```bash
# Main Website
cd am-with-emailjs && npm run build

# Admin Dashboard
cd am-with-emailjs/admin-dashboard/client && npm run build

# Backend Server (no build needed)
cd am-with-emailjs/admin-dashboard/server && npm start
```

### 📊 Port Configuration
```
Main Website Dev: 3000
Admin Dashboard Dev: 3001
Backend Server: 5000
MySQL Database: 3306
```

### 🎨 EmailJS Configuration (Contact Form)
```
Service ID: service_glf585p
Template ID: template_ideddtd
Public Key: g0FagqI_oJKBsprMA
```

---

## ⚠️ IMPORTANT: Update These Before Production

1. **Change admin password** from default
2. **Update all localhost URLs** to production domains
3. **Generate new JWT_SECRET** for production
4. **Set up production database** with strong password
5. **Configure CORS** with production domains only
6. **Enable HTTPS** on all domains
7. **Set up file storage** (S3/Cloudinary) for uploads
8. **Configure error monitoring** (Sentry/LogRocket)
9. **Set up database backups**
10. **Test email delivery** in production

---

## 📝 Environment Variables Template

### Backend (.env)
```env
# Database
DB_HOST=your-production-db-host
DB_USER=your-db-username
DB_PASSWORD=your-strong-password
DB_NAME=ecommerce_admin
DB_PORT=3306

# Server
PORT=5000
NODE_ENV=production

# Security
JWT_SECRET=your-generated-secret-key-here

# Email
EMAIL_USER=madasumiteesh@gmail.com
EMAIL_PASSWORD=mnfc xdxe ojpi rtzf
ADMIN_EMAIL=madasumiteesh@gmail.com

# Frontend URLs
FRONTEND_URL=https://your-domain.com
ADMIN_URL=https://admin.your-domain.com
```

### Frontend (.env)
```env
REACT_APP_API_URL=https://api.your-domain.com/api
```

---

## 🚀 Recommended Hosting Stack

### Free/Low-Cost Option:
- **Frontend**: Vercel (Free tier)
- **Admin Dashboard**: Vercel (Free tier)
- **Backend**: Railway (Free tier with credit card)
- **Database**: Railway MySQL (Free tier)
- **File Storage**: Cloudinary (Free tier)

### Professional Option:
- **Frontend**: Vercel Pro
- **Admin Dashboard**: Vercel Pro
- **Backend**: DigitalOcean Droplet ($6/month)
- **Database**: DigitalOcean Managed MySQL ($15/month)
- **File Storage**: AWS S3 (Pay as you go)
- **Email**: SendGrid (Free tier: 100 emails/day)

---

## 📞 Support Contacts

**Developer Support**: Available via email
**Business Contact**: madasumiteesh@gmail.com
**WhatsApp**: +91 91009 11697

---

**Last Updated**: February 2026
**Version**: 1.0.0
**Status**: Production Ready ✅
