# Glass Website 🥽

A modern, responsive eyewear e-commerce website showcasing premium optical and sunglasses collections. Built with Vite, EJS templating, and SCSS for a sleek and professional user experience.

## 🌟 Features

- **Product Showcases**: Comprehensive displays of optical glasses and sunglasses collections
- **Store Locator**: Interactive store locations with contact information and maps
- **Customer Reviews**: Testimonials and recommendations from satisfied customers
- **FAQ Section**: Comprehensive frequently asked questions about products and services
- **Blog**: Latest news and updates about eyewear trends
- **Responsive Design**: Fully optimized for desktop, tablet, and mobile devices
- **Professional UI**: Clean, modern design with smooth animations and transitions

## 🚀 Live Demo

Visit the live website: [https://j-i-p.github.io/glass_website/](https://j-i-p.github.io/glass_website/)

## 🛠️ Technology Stack

- **Build Tool**: Vite 4.2+
- **Templating**: EJS (Embedded JavaScript)
- **Styling**: SCSS/Sass
- **JavaScript**: ES6+ Modules
- **Fonts**: Google Fonts (Noto Sans TC, Roboto)
- **Icons**: Material Symbols
- **Deployment**: GitHub Pages

## 📋 Prerequisites

- Node.js version 16 or higher
- npm or yarn package manager

Check your Node.js version:
```bash
node -v
```

## ⚡ Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/J-I-P/glass_website.git
   cd glass_website
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```
   The site will open automatically in your browser at `http://localhost:5173/glass_website/pages/index.html`

4. **Build for production**
   ```bash
   npm run build
   ```

## 📁 Project Structure

```
glass_website/
├── assets/                 # Static assets
│   ├── images/            # Product images, icons, and graphics
│   └── scss/              # SCSS stylesheets
│       ├── base/          # Base styles, variables, reset
│       ├── layout/        # Header, footer, navigation styles
│       └── pages/         # Page-specific styles
├── layout/                # EJS template partials
│   ├── header.ejs         # Site header and navigation
│   ├── footer.ejs         # Site footer
│   └── *.ejs              # Other reusable components
├── pages/                 # HTML pages
│   ├── index.html         # Homepage
│   ├── classic-optical.html    # Optical glasses collection
│   ├── classic-sunglasses.html # Sunglasses collection
│   ├── location.html      # Store locations
│   ├── store-page.html    # Individual store details
│   ├── faq.html          # Frequently asked questions
│   └── blog.html         # Blog page
├── main.js               # Main JavaScript entry point
├── vite.config.js        # Vite configuration
└── package.json          # Project dependencies and scripts
```

## 🎯 Available Pages

- **Homepage** (`/`) - Main landing page with hero banner and product highlights
- **Classic Optical** (`/classic-optical.html`) - Prescription glasses collection
- **Classic Sunglasses** (`/classic-sunglasses.html`) - Sunglasses collection with color options
- **Store Locations** (`/location.html`) - Find nearby stores with contact information
- **Store Details** (`/store-page.html`) - Individual store information and maps
- **FAQ** (`/faq.html`) - Common questions about products and services
- **Blog** (`/blog.html`) - Latest news and eyewear trends

## 📱 Responsive Design

The website is fully responsive and optimized for:
- **Desktop**: 1200px and above
- **Tablet**: 768px - 1199px
- **Mobile**: 320px - 767px

## 🚀 Deployment

### Automatic Deployment to GitHub Pages

1. **Initial setup** (if not already done):
   ```bash
   git init
   git add .
   git commit -m 'Initial commit'
   git branch -M main
   git remote add origin [Your GitHub Repository URL]
   git push -u origin main
   ```

2. **Deploy to GitHub Pages**:
   ```bash
   npm run deploy
   ```

This will build the project and automatically deploy it to GitHub Pages.

### Manual Deployment

1. Build the project:
   ```bash
   npm run build
   ```

2. Upload the `dist` folder contents to your hosting provider.

## 🎨 Customization

### Colors and Branding

Edit the SCSS variables in `assets/scss/base/_variable.scss`:

```scss
$primary-color: #AA0601;      // Main brand color
$secondary-color: #FBF2F2;    // Secondary background
$title-color: #650300;        // Title color
```

### Content Management

- **Product Images**: Add new images to `assets/images/`
- **Store Information**: Edit store details in `pages/location.html` and `pages/store-page.html`
- **FAQ Content**: Update questions and answers in `pages/faq.html`
- **Navigation**: Modify the menu in `layout/header.ejs`

## 🔧 Development

### Available Scripts

- `npm run dev` - Start development server with hot reload
- `npm run build` - Build for production
- `npm run preview` - Preview production build locally
- `npm run deploy` - Build and deploy to GitHub Pages

### Development Features

- **Hot Reload**: Automatic page refresh on file changes
- **SCSS Compilation**: Real-time SCSS to CSS compilation
- **EJS Templating**: Reusable components and layouts
- **Asset Optimization**: Automatic image and file optimization during build

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

**Yi-Ping Jiang**
- Email: apple80177@gmail.com
- GitHub: [@J-I-P](https://github.com/J-I-P)

## 🙏 Acknowledgments

- Google Fonts for typography
- Material Design Icons for iconography
- Vite team for the excellent build tool
- Contributors and reviewers
