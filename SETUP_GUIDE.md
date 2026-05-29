# Website Setup Guide - Law Office of Peter K. Hoffmann

Your professional website is ready! Follow these simple steps to get it live.

## Step 1: Set Up Contact Form (Free with Formspree)

1. Go to **formspree.io** and sign up (it's free)
2. Create a new form and enter your email: **pkh@pkhlaw.com**
3. Formspree will give you a form ID (something like `abc123def`)
4. In the `index.html` file, find this line:
   ```
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
5. Replace `YOUR_FORM_ID` with the ID from Formspree
6. Test the form - Formspree will send you a confirmation email to verify

## Step 2: Choose Your Hosting (Both are Free)

### Option A: GitHub Pages (Recommended - Most Reliable)

1. Create a GitHub account at **github.com** (free)
2. Create a new repository named `pkhlaw.com` (or any name you prefer)
3. Upload your `index.html` file to the repository
4. Go to Settings → Pages → select "Deploy from a branch"
5. Your site will be available at `https://yourusername.github.io/pkhlaw.com`
6. GitHub Pages is very reliable and free forever

### Option B: Netlify (Easiest - Drag & Drop)

1. Go to **netlify.com** and sign up with GitHub (free)
2. Click "Add new site" → "Deploy manually"
3. Drag and drop your `index.html` file
4. Your site goes live instantly
5. You can customize the URL in site settings
6. Free tier includes unlimited sites

## Step 3: Point Your Domain to Your Website

You have your domain `pkhlaw.com` on GoDaddy. Update the DNS to point to your hosting:

### If using GitHub Pages:

1. Log into GoDaddy
2. Go to your domain settings → DNS
3. Find the DNS records section
4. Add these records:
   - Type: **CNAME**, Name: **www**, Value: `yourusername.github.io`
   - Type: **A**, Name: **@**, Value: `185.199.108.153` (GitHub's IP)
5. Wait 24-48 hours for DNS to update

### If using Netlify:

1. Log into Netlify and go to your site settings
2. Copy the Netlify URL (usually `something.netlify.app`)
3. In GoDaddy DNS settings, create a CNAME record:
   - Name: **www**
   - Value: `[your-netlify-url]`
4. Or use Netlify's simpler method: they'll guide you through it

## Step 4: Test Your Website

Once DNS updates (24-48 hours), visit **pkhlaw.com** and verify:
- ✅ Site loads correctly
- ✅ All pages display properly
- ✅ Contact form works
- ✅ Mobile looks good (test on phone)

## Ongoing Maintenance

Your website is static HTML - very easy to maintain:

- **To update text**: Edit `index.html` in any text editor
- **To add a new section**: Copy/paste a section block and modify
- **To add images**: You can add them later (I kept the design clean and image-free for now)
- **No database**: Nothing to back up or maintain
- **Fully yours**: No platform lock-in, you own the code

## Cost Summary

- Domain: Already have it ($0 - ongoing GoDaddy renewal)
- Hosting: **$0/month** (GitHub Pages or Netlify free tier)
- Contact form: **$0/month** (Formspree free tier, upgrade only if 50+ submissions/month)
- **Total: $0/month** ✅

## Questions?

If you run into any issues with these steps, let me know and I'll help you troubleshoot.

---

**Your website design includes:**
- Professional, modern layout
- Mobile-responsive (looks great on phones)
- Fast loading
- Clean, trustworthy design appropriate for law firm
- Contact form that emails you directly
- All your credentials and practice info prominently displayed
