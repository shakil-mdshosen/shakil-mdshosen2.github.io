# shakil-mdshosen.github.io

Personal website hosted on GitHub Pages with custom domain: **http://shakil.live/**

## 🌐 Custom Domain Setup

This repository is configured to use the custom domain `shakil.live` through GitHub Pages. The `CNAME` file contains the domain configuration.

### DNS Configuration Required

To make your domain work, you need to configure DNS settings at your domain registrar (name.com):

#### Option 1: Using A Records (Recommended for root domain)
Add these A records for `shakil.live`:
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

#### Option 2: Using CNAME (for www subdomain)
Add a CNAME record:
```
www.shakil.live → shakil-mdshosen.github.io
```

### GitHub Pages Settings
1. Go to your repository settings
2. Navigate to "Pages" section
3. Ensure "Source" is set to "Deploy from a branch"
4. Select "main" branch and "/ (root)" folder
5. The custom domain should show `shakil.live`
6. Enable "Enforce HTTPS" once DNS propagation is complete (24-48 hours)

## 📧 Free Email Hosting Options

Since you want free email for your domain `shakil.live`, here are the best options:

### Option 1: Zoho Mail (Recommended - Completely Free)

**Features:**
- 5GB storage per user
- Up to 5 users free
- Web interface and mobile apps
- IMAP/POP3 support

**Setup Steps:**
1. Sign up at [zoho.com/mail](https://zoho.com/mail)
2. Choose "Add your existing domain"
3. Enter `shakil.live`
4. Verify domain ownership
5. Add these DNS records at name.com:

**MX Records:**
```
Priority 10: mx.zoho.com
Priority 20: mx2.zoho.com
Priority 50: mx3.zoho.com
```

**TXT Record for verification:**
```
zoho-verification=<verification-code-provided-by-zoho>
```

**CNAME Records (optional but recommended):**
```
mail.shakil.live → business.zoho.com
```

### Option 2: Gmail with Custom Domain (Google Workspace - 14-day free trial, then paid)

**Note:** Google no longer offers free Gmail with custom domains, but you get a 14-day trial.

### Option 3: Email Forwarding (Free but limited)

**Setup email forwarding to your existing email:**

1. **At name.com (if they offer email forwarding):**
   - Set up forwarding from `you@shakil.live` to your existing email
   - Add MX records provided by name.com

2. **Using Cloudflare (Free):**
   - Transfer DNS management to Cloudflare (free)
   - Use Cloudflare Email Routing (free email forwarding)
   - Forward unlimited emails from your domain to existing email addresses

### Option 4: ProtonMail Custom Domain
- Offers custom domain email
- Privacy-focused
- Has free tier with limitations
- Paid plans for full custom domain features

## 🚀 Deployment

This site automatically deploys when you push changes to the main branch. The deployment process:

1. Push code to main branch
2. GitHub Actions builds and deploys the site
3. Changes appear at `https://shakil.live` (once DNS is configured)

## 📁 File Structure

```
├── CNAME              # Custom domain configuration
├── index.html         # Main website file
├── README.md          # This documentation
└── .git/              # Git repository data
```

## 🛠️ Development

To develop locally:
1. Clone this repository
2. Make changes to `index.html` or add new files
3. Test locally by opening `index.html` in a browser
4. Commit and push changes to deploy

## ⚠️ Important Notes

1. **DNS Propagation:** DNS changes can take 24-48 hours to propagate globally
2. **HTTPS:** Enable "Enforce HTTPS" in GitHub Pages settings only after DNS is working
3. **Email Setup:** Choose one email option and configure DNS records accordingly
4. **Domain Verification:** Some email providers require domain verification via TXT records

## 🆘 Troubleshooting

### Domain not working?
- Check DNS settings at name.com
- Wait for DNS propagation (up to 48 hours)
- Verify GitHub Pages settings

### Email not working?
- Verify MX records are correctly set
- Check spam folder for verification emails
- Ensure TXT verification records are added

### SSL Certificate issues?
- Wait for DNS propagation before enabling HTTPS
- GitHub automatically provisions SSL certificates for custom domains

## 📞 Support

For domain-related issues, contact name.com support.
For email hosting issues, contact your chosen email provider.
For GitHub Pages issues, check [GitHub Pages documentation](https://docs.github.com/en/pages).
