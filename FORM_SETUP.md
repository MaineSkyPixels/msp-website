# 📝 Contact Form Setup Guide

## Formspree Integration

Your contact form is now configured to work with **Formspree**, a reliable form handling service that works perfectly with static sites like Cloudflare Pages.

## 🚀 Quick Setup (5 minutes)

### Step 1: Create Formspree Account
1. Go to [formspree.io](https://formspree.io)
2. Click "Get Started" (free plan available)
3. Sign up with your email or GitHub account

### Step 2: Create New Form
1. After signing in, click "New Form"
2. Fill in the form details:
   - **Form Name**: "Maine Sky Pixels Contact"
   - **Email**: `info@maineskypixels.com` (or your preferred email)
3. Click "Create Form"

### Step 3: Get Your Form ID
1. After creating the form, you'll see a form endpoint URL like:
   ```
   https://formspree.io/f/xpzgkqwe
   ```
2. Copy the form ID (the part after `/f/`): `xpzgkqwe`

### Step 4: Update Your Website
1. Open `index.html` in your code editor
2. Find this line:
   ```html
   <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
3. Replace `YOUR_FORM_ID` with your actual form ID:
   ```html
   <form class="contact-form" action="https://formspree.io/f/xpzgkqwe" method="POST">
   ```

### Step 5: Update Success URL
1. In the same file, find this line:
   ```html
   <input type="hidden" name="_next" value="https://maineskypixels.pages.dev/?success=true">
   ```
2. Replace `maineskypixels.pages.dev` with your actual Cloudflare Pages URL

### Step 6: Deploy Changes
```bash
git add index.html
git commit -m "Configure contact form with Formspree"
git push origin main
```

## ✅ That's It!

Your contact form will now:
- ✅ Send emails to `info@maineskypixels.com`
- ✅ Show success/error messages
- ✅ Prevent spam with honeypot field
- ✅ Work on all devices
- ✅ Handle form validation

## 📧 Form Features

### What happens when someone submits:
1. **Client-side validation** - Checks required fields and email format
2. **Form submission** - Sends data to Formspree
3. **Email delivery** - You receive an email with the form data
4. **Success message** - User sees confirmation message
5. **Spam protection** - Honeypot field prevents bots

### Email format you'll receive:
```
Subject: New Contact Form Submission - Maine Sky Pixels

Name: John Doe
Email: john@example.com
Phone: (555) 123-4567
Message: I'm interested in your drone services...

Reply to: john@example.com
```

## 🔧 Advanced Configuration (Optional)

### Customize Email Subject
In `index.html`, change:
```html
<input type="hidden" name="_subject" value="New Contact Form Submission - Maine Sky Pixels">
```

### Add More Fields
You can add more form fields by adding them to the HTML form. Formspree will automatically capture them.

### Spam Protection
The form includes:
- Honeypot field (invisible to users)
- Client-side validation
- Formspree's built-in spam filtering

## 🆓 Pricing

- **Free Plan**: 50 submissions/month
- **Paid Plans**: Start at $10/month for more submissions
- **Perfect for**: Small to medium businesses

## 🆘 Troubleshooting

### Form not sending emails:
1. Check that you replaced `YOUR_FORM_ID` with your actual form ID
2. Verify your Formspree account is active
3. Check spam folder for test emails

### Success message not showing:
1. Make sure the `_next` URL matches your live website URL
2. Check browser console for JavaScript errors

### Need help?
- Formspree Documentation: [help.formspree.io](https://help.formspree.io)
- Formspree Support: Available on all paid plans

## 🎉 Success!

Once configured, your contact form will be fully functional and you'll start receiving inquiries from potential customers!
