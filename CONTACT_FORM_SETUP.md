# Contact Form Setup Instructions

The contact form on `/contact.html` uses **FormSubmit.co** - a free form submission service that sends emails without requiring backend code.

## ✅ How It Works

1. Users fill out the contact form with their email, subject, and message
2. FormSubmit.co receives the form submission
3. The email is forwarded to **shakil@bnwp.org**

## 🔧 First-Time Activation Required

**Important:** The first time someone submits the contact form, FormSubmit will send a **confirmation email** to shakil@bnwp.org.

### Activation Steps:

1. Have someone submit a test message through the contact form at `https://shakil.live/contact.html`
2. Check the inbox for **shakil@bnwp.org**
3. Look for an email from FormSubmit.co with subject "Confirm your email address"
4. Click the confirmation link in the email
5. Once confirmed, all future form submissions will be delivered automatically!

## 📧 Email Features

- **Sender's email** is included so you can reply directly
- **Subject line** shows: "New message from shakil.live contact form"
- **Table format** for easy reading
- **No captcha** for better user experience
- **No API key required** - works immediately after activation

## 🔄 Alternative Email Services (if needed)

If you prefer a different service, here are alternatives:

### Web3Forms (requires free API key)
- Sign up at https://web3forms.com
- Get your access key
- Update the form action and add the access key

### Formspree (free tier: 50 submissions/month)
- Sign up at https://formspree.io
- Get your form endpoint
- Update the form action URL

## 🛠️ Testing

After activation, test the form by:
1. Visiting https://shakil.live/contact.html
2. Filling out the form with test data
3. Submitting it
4. Checking shakil@bnwp.org for the email

## 📝 Form Fields

The contact form includes:
- **Email** (required) - Sender's email address
- **Subject/Heading** (required) - Brief subject line
- **Message** (required) - Detailed message content

All fields are validated before submission.
