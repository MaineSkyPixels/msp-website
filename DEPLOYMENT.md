# 🚀 Cloudflare Pages Deployment Guide

## Quick Start

Your Maine Sky Pixels website is now ready for Cloudflare Pages deployment! Here's how to get it live:

## 📋 Prerequisites

- [ ] Cloudflare account (free at [cloudflare.com](https://cloudflare.com))
- [ ] Git repository (GitHub, GitLab, or Bitbucket)
- [ ] Your website files (already prepared ✅)

## 🔧 Step-by-Step Deployment

### 1. Push to Git Repository

First, push your code to a Git hosting service:

```bash
# Add your remote repository (replace with your actual repo URL)
git remote add origin https://github.com/yourusername/maineskypixels-website.git

# Push to main branch
git push -u origin main
```

**Popular Git Hosting Options:**
- **GitHub** (recommended): [github.com](https://github.com)
- **GitLab**: [gitlab.com](https://gitlab.com)
- **Bitbucket**: [bitbucket.org](https://bitbucket.org)

### 2. Deploy to Cloudflare Pages

1. **Go to Cloudflare Pages**
   - Visit [pages.cloudflare.com](https://pages.cloudflare.com)
   - Sign in with your Cloudflare account

2. **Create New Project**
   - Click "Create a project"
   - Click "Connect to Git"

3. **Connect Repository**
   - Select your Git provider (GitHub, GitLab, etc.)
   - Authorize Cloudflare to access your repositories
   - Select your `maineskypixels-website` repository

4. **Configure Build Settings**
   ```
   Framework preset: None (Static Site)
   Build command: (leave empty)
   Build output directory: / (root directory)
   Root directory: (leave empty)
   ```

5. **Deploy**
   - Click "Save and Deploy"
   - Wait for deployment to complete (usually 1-2 minutes)

### 3. Custom Domain (Optional)

1. **Add Custom Domain**
   - In your Cloudflare Pages dashboard
   - Go to your project → "Custom domains"
   - Click "Set up a custom domain"
   - Enter your domain (e.g., `maineskypixels.com`)

2. **DNS Configuration**
   - Follow Cloudflare's DNS setup instructions
   - Add the required CNAME record to your domain registrar

## 🌐 Your Live Website

Once deployed, your website will be available at:
- **Cloudflare Pages URL**: `https://your-project-name.pages.dev`
- **Custom Domain**: `https://yourdomain.com` (if configured)

## 🔄 Updates and Maintenance

To update your website:

1. **Make Changes**
   ```bash
   # Edit your files locally
   # Test changes by opening index.html in browser
   ```

2. **Deploy Updates**
   ```bash
   git add .
   git commit -m "Update website content"
   git push origin main
   ```

3. **Automatic Deployment**
   - Cloudflare Pages automatically rebuilds and deploys
   - Changes go live in 1-2 minutes

## 📊 Performance Features

Your website includes these optimizations:

- ✅ **Fast Loading**: Optimized CSS and JavaScript
- ✅ **Mobile Responsive**: Works on all devices
- ✅ **SEO Optimized**: Meta tags and semantic HTML
- ✅ **CDN Delivery**: Cloudflare's global CDN
- ✅ **HTTPS**: Automatic SSL certificate
- ✅ **Caching**: Optimized for speed

## 🛠️ Troubleshooting

### Common Issues:

**Build Fails:**
- Check that build output directory is set to `/` (root)
- Ensure all files are committed to git

**Custom Domain Not Working:**
- Verify DNS records are correctly set
- Wait up to 24 hours for DNS propagation

**Styling Issues:**
- Clear browser cache
- Check that all CSS files are in the root directory

### Getting Help:

- **Cloudflare Support**: [support.cloudflare.com](https://support.cloudflare.com)
- **Documentation**: [developers.cloudflare.com/pages](https://developers.cloudflare.com/pages)

## 📈 Next Steps

After deployment, consider:

1. **Analytics**: Add Google Analytics or Cloudflare Analytics
2. **Contact Form**: Set up form handling (Formspree, Netlify Forms, etc.)
3. **SSL**: Verify HTTPS is working
4. **Performance**: Monitor Core Web Vitals in Cloudflare dashboard

## 🎉 Success!

Your Maine Sky Pixels website is now live and ready to serve customers!

**Contact Information:**
- Phone: (207) 200-1232
- Email: info@maineskypixels.com
- License: #10062506
