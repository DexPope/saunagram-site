# Saunagram - Instagram-Style E-commerce for Saunas & Wellness

A modern, Instagram-inspired e-commerce website for premium saunas and wellness products. Built as a single-page application with vanilla HTML, CSS, and JavaScript.

## 🔥 Features

### Instagram-Style Design
- **Profile Section**: Clean header with logo, bio, and stats (150+ Products, 5,000+ Happy Customers, ⭐ 4.9 Rating)
- **Stories Bar**: Horizontally scrollable category navigation with Instagram-style circles
- **Product Feed**: Toggle between grid view (like IG profile) and list view (like IG posts)
- **Product Modals**: Instagram post-style overlay with product details
- **Mobile-First**: Responsive design with bottom navigation on mobile

### E-commerce Functionality
- **15 Premium Products**: Across saunas, cold plunge, infrared, and accessories categories
- **Wishlist**: localStorage-based favorites system
- **Search**: Real-time product search
- **Category Filtering**: Filter products by category without page reload
- **Affiliate Ready**: Product data includes affiliate URL fields (currently placeholder "#")

### Categories
- 🔥 Saunas
- ❄️ Cold Plunge
- 🌡️ Infrared
- 💆 Spa & Massage
- 🧴 Accessories
- 🏋️ Recovery
- ⭐ Best Sellers
- 🏷️ Sale

### Product Range
**High-Ticket Items ($199 - $6,799):**
- Outdoor Barrel Sauna 4-Person ($4,299)
- Traditional Finnish Sauna Kit ($6,799)
- Cold Plunge Chiller Unit ($2,999)
- Indoor Infrared Sauna 2-Person ($2,199)
- Ice Bath Cold Plunge Tub ($1,499)

**Accessories ($24 - $79):**
- Sauna Hat (Wool) ($24)
- Sauna Thermometer & Hygrometer ($39)
- Essential Oil Sauna Kit ($49)
- Cedar Sauna Bucket & Ladle Set ($69)
- Premium Sauna Stones 40lbs ($79)

## 🚀 Deployment

### GitHub Pages Setup

1. **Create GitHub Repository**
   ```bash
   # Create a new repository on GitHub named "saunagram-site"
   # Make sure it's public for GitHub Pages
   ```

2. **Push to GitHub**
   ```bash
   git remote add origin https://github.com/yourusername/saunagram-site.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to repository Settings
   - Scroll to Pages section
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Save settings

4. **Custom Domain (Optional)**
   - The CNAME file is already configured for `saunagram.shop`
   - Add DNS records for your domain:
     - Type: CNAME
     - Host: www
     - Value: yourusername.github.io
   - Wait for DNS propagation (up to 48 hours)

### Alternative Hosting
- **Netlify**: Drag and drop the entire folder
- **Vercel**: Connect GitHub repository
- **Firebase Hosting**: Use Firebase CLI
- **Any Static Host**: Upload all files to web root

## 🛠️ Customization

### Adding Products
Edit the `products` array in the JavaScript section:

```javascript
{
    id: 16,
    name: "New Product Name",
    brand: "Brand Name",
    price: 1299,
    originalPrice: 1599, // Optional for sale items
    category: "saunas", // saunas, cold-plunge, infrared, accessories
    image: "https://images.unsplash.com/photo-XXXXX?w=600&h=600&fit=crop",
    description: "Product description...",
    features: [
        "Feature 1",
        "Feature 2",
        "Feature 3"
    ],
    affiliateUrl: "https://your-affiliate-link.com"
}
```

### Updating Affiliate Links
Replace the `affiliateUrl: "#"` placeholder with your actual affiliate links:

```javascript
// Find the product and update:
affiliateUrl: "https://partner.example.com/product?ref=yourcode"
```

### Customizing Colors
The Instagram gradient can be customized in the CSS:

```css
/* Main gradient */
background: linear-gradient(45deg, #F56040, #FFAD46, #FFDD59);

/* Custom gradient */
background: linear-gradient(45deg, #your-color1, #your-color2, #your-color3);
```

### Adding Categories
Add to the `categories` array:

```javascript
{ id: 'new-category', name: 'New Category', icon: '🆕' }
```

## 📱 Technical Details

### Performance
- **Single HTML File**: No external dependencies for fast loading
- **Optimized Images**: Uses Unsplash CDN with proper sizing (`w=600&h=600&fit=crop`)
- **Lazy Loading**: Images load as needed
- **localStorage**: Wishlist data persists across sessions

### Browser Support
- **Modern Browsers**: Chrome, Firefox, Safari, Edge (ES6+ features used)
- **Mobile**: Responsive design works on all screen sizes
- **PWA Ready**: Can be extended to Progressive Web App

### SEO Optimized
- Semantic HTML structure
- Meta tags for social sharing
- Descriptive alt tags for images
- Clean URL structure

## 🔧 Development

### Local Development
1. Open `index.html` in any modern browser
2. Use a local server for best experience:
   ```bash
   # Python
   python -m http.server 8000
   
   # Node.js
   npx http-server
   
   # PHP
   php -S localhost:8000
   ```

### File Structure
```
saunagram-site/
├── index.html          # Complete website (HTML + CSS + JS)
├── CNAME               # GitHub Pages custom domain
├── README.md           # This file
└── .git/               # Git repository
```

## 🎨 Design Philosophy

**Instagram Aesthetic**
- Clean white backgrounds (#FAFAFA)
- Subtle gray borders (#DBDBDB)
- Instagram gradient accents
- System font stack (-apple-system)
- Rounded corners and subtle shadows
- Mobile-first responsive design

**E-commerce UX**
- Familiar Instagram navigation patterns
- Quick product discovery through stories/categories
- Seamless grid-to-detail transitions
- One-click wishlist management
- Search-as-you-type functionality

## 📈 Future Enhancements

### Phase 2 Features
- [ ] Product reviews and ratings
- [ ] Shopping cart functionality
- [ ] User accounts and login
- [ ] Email newsletter signup
- [ ] Product recommendations
- [ ] Social media integration

### Phase 3 Features
- [ ] Inventory management
- [ ] Order tracking
- [ ] Live chat support
- [ ] Advanced filtering (price, brand, features)
- [ ] Product comparison
- [ ] Dealer/installer locator

## 🔗 Links

- **Live Site**: https://saunagram.shop (after deployment)
- **Repository**: https://github.com/yourusername/saunagram-site

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

**Built with ❤️ for the sauna and wellness community**

*Ready to deploy and start selling premium wellness products with an Instagram-style shopping experience.*