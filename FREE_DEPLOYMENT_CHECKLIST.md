# ✅ FREE Deployment Checklist ($0/month)

---

## 🗄️ Step 1: Free MySQL Database (Clever Cloud)

- [ ] Created Clever Cloud account (no credit card needed)
- [ ] Created MySQL add-on (DEV plan - FREE)
- [ ] Copied connection details:
  - [ ] MYSQL_ADDON_HOST: `_______________________________`
  - [ ] MYSQL_ADDON_USER: `_______________________________`
  - [ ] MYSQL_ADDON_PASSWORD: `_______________________________`
  - [ ] MYSQL_ADDON_DB: `_______________________________`
  - [ ] MYSQL_ADDON_PORT: `_______________________________`
- [ ] Imported database schema (`complete_setup.sql`)
- [ ] Imported seed data (`seed.sql`)
- [ ] Tested connection

---

## 🔧 Step 2: Backend API (Render - FREE)

- [ ] Created Render account (sign in with GitHub)
- [ ] Created new Web Service
- [ ] Connected GitHub repository
- [ ] Set Root Directory: `admin-dashboard/server`
- [ ] Set Build Command: `npm install`
- [ ] Set Start Command: `npm start`
- [ ] Selected FREE instance type
- [ ] Added environment variables (11 total):
  - [ ] DB_HOST (from Clever Cloud)
  - [ ] DB_USER (from Clever Cloud)
  - [ ] DB_PASSWORD (from Clever Cloud)
  - [ ] DB_NAME (from Clever Cloud)
  - [ ] DB_PORT (from Clever Cloud)
  - [ ] PORT = 5000
  - [ ] NODE_ENV = production
  - [ ] JWT_SECRET (generated random string)
  - [ ] EMAIL_USER
  - [ ] EMAIL_PASSWORD
  - [ ] ADMIN_EMAIL
- [ ] Deployment successful
- [ ] Backend URL: `_______________________________`
- [ ] Tested: `/api/health` returns OK

---

## 🌐 Step 3: Main Website (Vercel - FREE)

- [ ] Updated `.env.production` with backend URL
- [ ] Committed and pushed to GitHub
- [ ] Created Vercel account (sign in with GitHub)
- [ ] Imported GitHub repository
- [ ] Set Framework: Create React App
- [ ] Set Root Directory: blank
- [ ] Added environment variable: `REACT_APP_API_URL`
- [ ] Deployment successful
- [ ] Website URL: `_______________________________`
- [ ] Tested website works

---

## 👨‍💼 Step 4: Admin Dashboard (Vercel - FREE)

- [ ] Updated `admin-dashboard/client/.env.production`
- [ ] Committed and pushed to GitHub
- [ ] Created new Vercel project (same repo)
- [ ] Set Framework: Vite
- [ ] Set Root Directory: `admin-dashboard/client`
- [ ] Added environment variable: `VITE_API_URL`
- [ ] Deployment successful
- [ ] Admin URL: `_______________________________`
- [ ] Tested admin dashboard works

---

## 🔄 Step 5: Update CORS

- [ ] Updated FRONTEND_URL in Render (actual Vercel URL)
- [ ] Updated ADMIN_URL in Render (actual Vercel URL)
- [ ] Backend redeployed automatically
- [ ] No CORS errors in browser console

---

## 🎯 Step 6: Final Testing

- [ ] Customer can browse products
- [ ] Customer can add to cart
- [ ] Customer can place order
- [ ] Customer can upload payment screenshot
- [ ] Order confirmation email received
- [ ] Admin can request login
- [ ] Admin receives approval email
- [ ] Admin can approve login
- [ ] Admin can view dashboard
- [ ] Admin can see payment verifications
- [ ] All features working

---

## 🚀 Optional: Keep Backend Awake

- [ ] Created UptimeRobot account (free)
- [ ] Added monitor for backend health endpoint
- [ ] Set check interval: 5 minutes
- [ ] Backend stays awake (no 30-second delay)

---

## 📊 Your FREE Deployment

```
Main Website:     https://________________________________
Admin Dashboard:  https://________________________________
Backend API:      https://________________________________
Database:         Clever Cloud MySQL (FREE)
Keep-Alive:       UptimeRobot (FREE)

Total Cost:       $0/month ✅
```

---

## 💡 Important Notes

### Render FREE Tier:
- ⚠️ Sleeps after 15 minutes of inactivity
- ⚠️ First request takes 30-60 seconds to wake
- ✅ Use UptimeRobot to keep it awake
- ✅ 750 hours/month (more than enough)

### Clever Cloud FREE Tier:
- ✅ 256MB storage
- ✅ Perfect for small projects
- ✅ No credit card required

### Vercel FREE Tier:
- ✅ Unlimited projects
- ✅ 100GB bandwidth/month
- ✅ Automatic SSL
- ✅ Global CDN

---

## 🔒 Security Checklist

- [ ] Changed JWT_SECRET to random string
- [ ] Verified `.env` files not in git
- [ ] All environment variables set correctly
- [ ] Database credentials secure
- [ ] Email credentials working

---

## 📝 Backup Plan

- [ ] Exported database backup
- [ ] Saved backup file: `_______________________________`
- [ ] Tested restore process
- [ ] Set reminder for weekly backups

---

## 🆘 Quick Troubleshooting

**Backend slow on first request?**
→ Normal! Render is waking up (30-60 seconds)
→ Set up UptimeRobot to keep it awake

**CORS errors?**
→ Check FRONTEND_URL and ADMIN_URL in Render
→ Make sure they match your Vercel URLs exactly

**Database connection failed?**
→ Verify all 5 Clever Cloud variables
→ Check database is active in Clever Cloud dashboard

**Build failed on Vercel?**
→ Check build logs
→ Try deploying again

---

## 🎉 Success!

- [ ] All services deployed
- [ ] All features tested
- [ ] No errors in console
- [ ] Emails working
- [ ] Ready for customers!

**Date Completed: _______________**

**Total Cost: $0/month** 💰

---

## 📞 Support

Full Guide: `FREE_DEPLOYMENT_GUIDE.md`
Email: madasumiteesh@gmail.com

**Congratulations on your FREE deployment! 🚀**
