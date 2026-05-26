# Contact Form Setup Instructions

## Web3Forms Configuration

The contact forms on your website use **Web3Forms** for spam-protected email delivery. To activate the forms, you need to get a free API key.

### Steps to Activate Forms:

1. **Get Your Free API Key:**
   - Go to https://web3forms.com/
   - Click "Get Started Free"
   - Enter your email: **estimates@burchcontracting.com**
   - Verify your email
   - Copy your Access Key

2. **Update index.html:**
   - Open `index.html` in your editor
   - Search for: `YOUR_WEB3FORMS_KEY_HERE` (appears twice)
   - Replace both instances with your actual API key

3. **Test the Forms:**
   - After updating and deploying, visit your site
   - Fill out the contact form
   - Submit and check estimates@burchcontracting.com for the test email

### Form Locations:

- **Hero Form** (top of page) - Line ~542
- **Contact Section** (dedicated contact page) - Line ~1005

### Spam Protection Features:

✅ **Honeypot Field** - Hidden checkbox that bots typically fill out  
✅ **Time Validation** - Prevents instant bot submissions (3 second minimum)  
✅ **Email Validation** - Ensures valid email format  
✅ **Required Fields** - Name, email, phone, project type must be filled  

### Alternative: Use Formspree

If you prefer Formspree instead:
1. Sign up at https://formspree.io/
2. Get your form endpoint URL
3. Replace `https://api.web3forms.com/submit` with your Formspree endpoint
4. Remove the `access_key` hidden input fields

### Fallback Contact

If forms don't work, all CTAs also link to:
- Phone: (864) 724-4600
- Email: estimates@burchcontracting.com

---

## Additional CTA Buttons Added:

- ✅ Service cards (3 locations) - Call + Request Quote buttons
- ✅ Cost calculator - Call + Request Quote Online buttons  
- ✅ CTA Banner - Request Quote Online button
- ✅ Dedicated contact section with full form

All quote request buttons link to `#contact` which scrolls to the contact form.
