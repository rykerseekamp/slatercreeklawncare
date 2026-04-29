# Slater Creek Lawn Services Website

Professional single-page website for Slater Creek Lawn Services - serving Anna, Texas with reliable, high-quality lawn maintenance services.

![Slater Creek Lawn Services](assets/logo.png)

## Features

- **Modern, Responsive Design** - Beautiful on all devices with mobile hamburger menu
- **Sticky Navigation** - Easy access to all sections with phone number in navbar
- **Hero Section** - Eye-catching full-screen hero with lawn background
- **Services Showcase** - Professional icons highlighting key services
- **Transparent Pricing** - Clear pricing cards with best value badge
- **Service Area Map** - Google Maps integration showing Anna, TX location
- **Contact Form** - Web3Forms integration for email submissions
- **Smooth Animations** - Fade-in effects, hover animations, and scroll interactions
- **Professional Icons** - Font Awesome icons throughout

## Setup Instructions

### 1. Web3Forms Configuration

The contact form uses Web3Forms to send emails to your business email.

**Steps to configure:**

1. Go to [https://web3forms.com](https://web3forms.com)
2. Sign up for a free account
3. Create a new form and set the email to your business email
4. Copy your Access Key
5. In `index.html`, find line 833 and replace:
   ```html
   <input type="hidden" name="access_key" value="YOUR_WEB3FORMS_ACCESS_KEY">
   ```
   with your actual access key:
   ```html
   <input type="hidden" name="access_key" value="abc123-your-actual-key-here">
   ```

### 2. Google Maps Configuration (Optional)

The Service Area section currently uses a pre-configured Google Maps embed showing Anna, Texas. **This works without any API key!**

If you want to customize the map further (different zoom, style, etc.):

1. Go to [Google Maps](https://www.google.com/maps)
2. Search for "Anna, TX"
3. Click the "Share" button
4. Click "Embed a map"
5. Copy the iframe code
6. Replace the iframe in `index.html` (around line 836) with your custom embed code

**Note:** The current map works out of the box with no configuration needed!

### 3. Deploy to Vercel

1. Push this repository to GitHub (already done!)
2. Go to [https://vercel.com](https://vercel.com)
3. Click "New Project"
4. Import your GitHub repository: `slatercreeklawncare`
5. Vercel will auto-detect it as a static site
6. Click "Deploy"
7. Your site will be live at `https://your-project.vercel.app`

**Optional:** Add a custom domain in Vercel project settings.

## Project Structure

```
website/
â”œâ”€â”€ assets/
â”‚   â””â”€â”€ logo.png              # GreenEdge logo with transparency
â”œâ”€â”€ index.html                # Main website file (single-page)
â”œâ”€â”€ README.md                 # This file
â””â”€â”€ .claude/                  # Claude Code settings
```

## Customization

### Update Pricing
Find the pricing section around line 779-803 in `index.html`:
- One-Time Lawn Care: Currently `$35-$45`
- Bi-Weekly Plan: Currently `$30-$40`
- Weekly Plan: Currently `$25-$35`

### Change Colors
Color variables are defined in CSS (lines 19-27):
```css
--dark-green: #1a3d1a;
--darker-green: #0f2d0f;
--accent-green: #4caf50;
--bright-green: #6ecf35;
```

### Update Content
All content is in `index.html`. Sections are clearly labeled with comments:
- Hero Section (line 708)
- About Section (line 724)
- Services Section (line 751)
- Pricing Section (line 775)
- Service Area Section (line 818)
- Contact Section (line 843)
- Footer (line 890)

## Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with flexbox/grid, gradients, animations
- **Vanilla JavaScript** - Form handling, smooth scrolling, animations
- **Font Awesome 6** - Professional icons
- **Google Fonts** - Bebas Neue & Montserrat
- **Web3Forms** - Contact form backend
- **Google Maps Embed API** - Service area visualization

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance

- Minimal external dependencies
- Optimized images from Unsplash CDN
- Lazy loading for maps iframe
- Single HTML file for fast loading

## Contact

**Slater Creek Lawn Services**
- Phone: [267-449-5490](tel:267-449-5490)
- Location: Anna, Texas

**Operated by:** Ryker & Eli

---

*Built with [Claude Code](https://claude.com/claude-code)*
