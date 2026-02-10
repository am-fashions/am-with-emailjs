# EmailJS Setup Guide for Contact Form

## Steps to Configure EmailJS

### 1. Create an EmailJS Account
- Go to [https://www.emailjs.com/](https://www.emailjs.com/)
- Sign up for a free account

### 2. Add Email Service
- Go to **Email Services** in your dashboard
- Click **Add New Service**
- Choose your email provider (Gmail, Outlook, etc.)
- Follow the connection steps
- Note down your **Service ID**

### 3. Create Email Template
- Go to **Email Templates** in your dashboard
- Click **Create New Template**
- Use these template variables in your email template:
  ```
  From: {{from_name}}
  Email: {{from_email}}
  
  Message:
  {{message}}
  ```
- Save and note down your **Template ID**

### 4. Get Your Public Key
- Go to **Account** → **General**
- Find your **Public Key** (also called User ID)

### 5. Update the Contact.jsx File
Open `src/pages/Contact.jsx` and replace these values around line 17-19:

```javascript
const serviceId = 'YOUR_SERVICE_ID';      // Replace with your Service ID
const templateId = 'YOUR_TEMPLATE_ID';    // Replace with your Template ID
const publicKey = 'YOUR_PUBLIC_KEY';      // Replace with your Public Key
```

### 6. Test Your Form
- Run your development server: `npm start`
- Navigate to the Contact page
- Fill out and submit the form
- Check your email inbox for the message

## Example Template Configuration

**Template Name:** Contact Form Submission

**Subject:** New Contact Form Message from {{from_name}}

**Content:**
```
Hello AM Fashions Team,

You have received a new message from your website contact form.

Name: {{from_name}}
Email: {{from_email}}

Message:
{{message}}

---
This email was sent from your AM Fashions website contact form.
```

## Troubleshooting

- **Email not sending?** Check browser console for errors
- **Invalid credentials?** Double-check your Service ID, Template ID, and Public Key
- **Emails going to spam?** Add your domain to EmailJS allowed domains in settings

## Free Tier Limits
- 200 emails per month
- Upgrade to paid plan for more emails
