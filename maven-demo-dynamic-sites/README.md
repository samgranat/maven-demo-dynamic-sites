# Maven AI Demo Sites

A collection of industry-specific demo sites showcasing Maven AI's capabilities across different verticals. Each demo features user switching, data visualization, instant answers search, and responsive design.

## 🚀 Live Demos

- **Telecom (Televia)**: https://televia.netlify.app/
- **Travel (Aventra)**: _[Deploy to get URL]_
- **Financial (FlowFi)**: _[Deploy to get URL]_
- **B2B CRM (KikkoCRM)**: _[Deploy to get URL]_

## 📁 Demos Included

### 1. Travel - Aventra (`travel-aventra/`)
Premium travel booking experience with airline data.

**Features:**
- 10 demo users with unique flight assignments
- Real-time flight information (status, route, departure time)
- Seat class details (Business, Economy, Extra Legroom)
- Loyalty program status
- Scenic hero background with search
- Purple branding (#a598b6)

**User switcher:** jdoe0-jdoe9

### 2. Telecom - Televia (`telecom-televia/`)
Mobile carrier account dashboard.

**Features:**
- 3 demo users with different plans
- Data usage visualization with progress bar
- Plan details (price, lines, data allocation)
- Account information and location
- Satellite dish hero background
- Teal branding (#14b8a6)

**User switcher:** Jonathan, Sarah, Michael

### 3. Financial - FlowFi (`financial-flowfi/`)
Financial services customer portal.

**Features:**
- Account balance and transaction history
- Multiple payment methods
- Recent activity tracking
- Financial insights
- Professional navy/blue branding

### 4. B2B CRM - KikkoCRM (`b2b-kikkocrm/`)
B2B customer relationship management interface.

**Features:**
- Sales pipeline visualization
- Order history and box tracking
- Contact management
- Account details
- Professional CRM styling

## 🛠️ Technical Stack

- **Frontend:** Pure HTML, CSS, vanilla JavaScript
- **Fonts:** System fonts (system-ui, Segoe UI, Roboto, etc.)
- **Build:** None required - standalone files
- **Dependencies:** Zero
- **Browser Support:** All modern browsers (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)

## 📦 Deployment

### Quick Deploy to Netlify

1. Go to https://app.netlify.com/
2. Drag and drop any demo folder (e.g., `travel-aventra/`)
3. Get instant live URL

### Deploy to Other Hosts

All demos are static HTML - upload to any hosting service:
- Vercel
- GitHub Pages
- AWS S3
- Cloudflare Pages
- Any web server

### View Locally

No server needed - just open `index.html` in any browser:

```bash
cd travel-aventra
open index.html  # macOS
# or double-click index.html
```

## 🎨 Customization

### Changing User Data

Each demo has a `users` object in the JavaScript section:

```javascript
const users = {
    'jdoe0': { flightNumber: 'AD35', seatType: 'Business Class', ... },
    'jdoe1': { flightNumber: 'AD322', seatType: 'Economy', ... }
};
```

Edit this to customize demo data.

### Changing Brand Colors

Find the CSS variables in the `<style>` section:

```css
/* Travel - Purple */
border-left: 4px solid #a598b6;
background: #a598b6;

/* Telecom - Teal */
border-left: 4px solid #14b8a6;
background: #14b8a6;
```

### Updating Content

All text, images, and styling are in `index.html` - edit directly in any text editor.

## 📂 Repository Structure

```
maven-demos-repo/
├── README.md
├── travel-aventra/
│   ├── index.html
│   ├── aventra.svg
│   ├── aventra-background.jpg
│   └── aventra-background-2.jpg
├── telecom-televia/
│   ├── index.html
│   ├── televia-logo.svg
│   └── televia-background.jpg
├── financial-flowfi/
│   ├── index.html
│   └── [assets]
└── b2b-kikkocrm/
    ├── index.html
    └── [assets]
```

## 🎯 Common Features Across All Demos

✅ **User Switcher** - Toggle between demo users
✅ **Data Cards** - Display key information in grid layout
✅ **Instant Answers** - Search bar for knowledge base queries
✅ **Help Button** - Pill-shaped "Get Help" button (bottom-right)
✅ **Responsive Design** - Mobile, tablet, and desktop layouts
✅ **System Fonts** - Fast loading with native typography
✅ **No Build Required** - Pure HTML/CSS/JS

## 🔧 Development

### Prerequisites

None! These are static HTML files.

### Making Changes

1. Open `index.html` in your favorite editor
2. Make changes to HTML, CSS, or JavaScript
3. Save and refresh browser
4. Deploy when ready

### Adding New Demos

Follow the same structure:

```
new-demo/
├── index.html
└── assets/
    ├── logo.svg
    └── background.jpg
```

## 📝 Design System

### Typography
- **Font Stack:** `system-ui, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif`
- **Body Weight:** 400 (normal)
- **Headers:** 600-700
- **Hero Headings:** 300 (light)

### Layout
- **Container Max Width:** 1400px
- **Card Padding:** 30px
- **Grid Gap:** 25px
- **Border Radius:** 2px (cards), 50px (buttons)

### Colors by Vertical
- **Travel:** #a598b6 (Purple)
- **Telecom:** #14b8a6 (Teal)
- **Financial:** Navy/Blue tones
- **B2B:** Professional grays

## 🤝 Contributing

To add new features or demos:

1. Fork this repository
2. Create a feature branch
3. Make your changes
4. Test across browsers
5. Submit a pull request

## 📄 License

These demos are for demonstration purposes. Customize and deploy as needed.

## 📞 Support

For questions about Maven AI integration:
- Visit: https://maven.ai
- Docs: https://docs.maven.ai

---

**Built with Maven AI** | Last Updated: January 2026
