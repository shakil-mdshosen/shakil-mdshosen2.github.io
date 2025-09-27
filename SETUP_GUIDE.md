# Quick Setup Guide for shakil.live

## 🚀 Your website is ready! Here's how to make it live:

### Step 1: Enable GitHub Pages (2 minutes)
1. Go to your repository: https://github.com/shakil-mdshosen/shakil-mdshosen.github.io
2. Click **Settings** tab
3. Scroll down to **Pages** section
4. Under "Source", select **Deploy from a branch**
5. Choose **main** branch and **/ (root)** folder
6. Click **Save**

### Step 2: Configure DNS at name.com (5 minutes)
Login to your name.com account and add these DNS records:

**For root domain (shakil.live):**
```
Type: A Record
Host: @
Value: 185.199.108.153

Type: A Record  
Host: @
Value: 185.199.109.153

Type: A Record
Host: @  
Value: 185.199.110.153

Type: A Record
Host: @
Value: 185.199.111.153
```

**For www subdomain (optional):**
```
Type: CNAME
Host: www
Value: shakil-mdshosen.github.io
```

### Step 3: Wait for DNS Propagation (24-48 hours)
- DNS changes take time to propagate globally
- You can check status at: https://whatsmydns.net/#A/shakil.live

### Step 4: Enable HTTPS (after DNS works)
1. Return to GitHub Pages settings
2. Check **Enforce HTTPS** (only after domain works)

## 📧 Free Email Setup (Choose One)

### Option A: Zoho Mail (Recommended - 100% Free)
1. Sign up at https://zoho.com/mail
2. Add domain `shakil.live`
3. Add these MX records at name.com:
   ```
   Type: MX, Host: @, Value: mx.zoho.com, Priority: 10
   Type: MX, Host: @, Value: mx2.zoho.com, Priority: 20
   Type: MX, Host: @, Value: mx3.zoho.com, Priority: 50
   ```

### Option B: Email Forwarding via Cloudflare (Free)
1. Transfer DNS to Cloudflare (free)
2. Use Cloudflare Email Routing
3. Forward emails to your existing email

## ✅ Final Checklist
- [ ] GitHub Pages enabled
- [ ] DNS records added at name.com
- [ ] Wait 24-48 hours for propagation
- [ ] Test website at https://shakil.live
- [ ] Enable HTTPS in GitHub Pages
- [ ] Choose and setup email hosting
- [ ] Customize website content

## 🆘 Need Help?
- **DNS issues**: Contact name.com support
- **Email issues**: Contact your chosen email provider
- **GitHub Pages**: Check [GitHub Docs](https://docs.github.com/en/pages)

Your website will be live at https://shakil.live once DNS propagates! 🎉