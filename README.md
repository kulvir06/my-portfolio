# Kulvir Singh - Portfolio Website

A modern, responsive portfolio website built with HTML, CSS, and JavaScript, inspired by professional portfolio designs. This project is optimized for GitHub Pages deployment.

## 🚀 Features

- **Responsive Design**: Works perfectly on all devices (desktop, tablet, mobile)
- **Modern UI/UX**: Clean, professional design with smooth animations
- **Interactive Elements**: Portfolio filtering, contact modal, smooth scrolling
- **Mobile-First**: Optimized for mobile devices with hamburger navigation
- **Smooth Animations**: CSS animations and JavaScript-powered interactions
- **Contact Form**: Functional contact form with validation
- **Portfolio Showcase**: Filterable project gallery with categories
- **Professional Sections**: About, Resume, Portfolio, and Contact sections
- **GitHub Pages Ready**: Optimized for deployment on GitHub Pages

## 📁 File Structure

```
my-portfolio/
├── index.html              # Main HTML file (entry point for GitHub Pages)
├── styles.css              # CSS styles and responsive design
├── script.js               # JavaScript functionality
├── .nojekyll               # Disables Jekyll processing for GitHub Pages
├── .github/
│   └── workflows/
│       └── pages.yml       # GitHub Actions workflow for deployment
├── package.json            # Project configuration
└── README.md               # This file
```

## 🚀 GitHub Pages Deployment

### Prerequisites

1. **GitHub Account**: Make sure you have a GitHub account
2. **Repository**: Create a new repository or use an existing one
3. **Repository Visibility**: For GitHub Free accounts, the repository must be **public**

### Step-by-Step Deployment

#### 1. Create/Setup Repository

**Option A: New Repository**
1. Go to [GitHub](https://github.com) and click the "+" icon in the top right
2. Select "New repository"
3. Name your repository (e.g., `my-portfolio`, `portfolio`, or `username.github.io`)
4. Make it **public**
5. Check "Initialize this repository with a README"
6. Click "Create repository"

**Option B: Existing Repository**
1. Navigate to your existing repository
2. Make sure it's **public** (required for GitHub Free accounts)

#### 2. Upload Your Portfolio Files

**Option A: Using Git (Recommended)**
```bash
# Clone your repository
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name

# Copy your portfolio files to this directory
# (index.html, styles.css, script.js, .nojekyll, .github folder)

# Add all files
git add .

# Commit changes
git commit -m "Initial portfolio commit"

# Push to GitHub
git push origin main
```

**Option B: Using GitHub Web Interface**
1. Go to your repository on GitHub
2. Click "Add file" → "Upload files"
3. Drag and drop your portfolio files
4. Commit the changes

#### 3. Configure GitHub Pages

1. In your repository, go to **Settings** tab
2. In the left sidebar, click **Pages**
3. Under "Source", select **GitHub Actions**
4. The GitHub Actions workflow will automatically deploy your site

#### 4. View Your Published Site

1. After pushing your code, wait 2-5 minutes for deployment
2. Go to **Settings** → **Pages**
3. Click **Visit site** to view your portfolio
4. Your site will be available at: `https://yourusername.github.io/your-repo-name`

### Repository Naming Options

- **Project Site**: `your-repo-name` → `https://yourusername.github.io/your-repo-name`
- **User Site**: `yourusername.github.io` → `https://yourusername.github.io`
- **Organization Site**: `organizationname.github.io` → `https://organizationname.github.io`

## 🛠️ Local Development

### Quick Start
1. **Clone or Download**: Get the files to your local machine
2. **Open in Browser**: Simply open `index.html` in any modern web browser
3. **Local Development**: Use a local server for development (recommended)

### Using Local Server (Recommended)

```bash
# Using Python 3
python3 -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Using PHP
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

## 🎨 Customization Guide

### Personal Information

Edit the following sections in `index.html`:

#### Hero Section
```html
<h1 class="hero-title">Your Name</h1>
<p class="hero-subtitle">Your Title</p>
```

#### Contact Information
```html
<span>your.email@example.com</span>
<span>+1 (555) 123-4567</span>
<span>Your Birthday</span>
<span>Your Location</span>
```

#### Social Media Links
```html
<a href="https://github.com/yourusername" target="_blank" rel="noopener noreferrer">
<a href="https://linkedin.com/in/yourusername" target="_blank" rel="noopener noreferrer">
<a href="https://twitter.com/yourusername" target="_blank" rel="noopener noreferrer">
```

#### About Section
```html
<p class="about-text">
    Your personal description here...
</p>
```

#### Education & Experience
Update the timeline sections in the Resume section with your actual information.

#### Skills
Modify the skills categories to match your expertise.

#### Portfolio Projects
Add your own projects by duplicating the portfolio-item structure and updating:
- Project title
- Description
- Technology tags
- Category (for filtering)

### Styling Customization

#### Colors
Main colors are defined in `styles.css`:
```css
:root {
    --primary-color: #2563eb;
    --secondary-color: #667eea;
    --accent-color: #764ba2;
}
```

#### Fonts
Change the font family in `styles.css`:
```css
body {
    font-family: 'Your Font', sans-serif;
}
```

#### Backgrounds
Modify gradient backgrounds in the hero section and other elements.

### Adding Your Photo

Replace the placeholder icon in the hero section:
```html
<div class="profile-placeholder">
    <img src="path/to/your/photo.jpg" alt="Your Name" style="width: 100%; height: 100%; object-fit: cover; border-radius: 50%;">
</div>
```

## 📱 Responsive Breakpoints

- **Desktop**: 1200px and above
- **Tablet**: 768px - 1199px
- **Mobile**: Below 768px
- **Small Mobile**: Below 480px

## 🔧 JavaScript Features

- **Mobile Navigation**: Hamburger menu for mobile devices
- **Smooth Scrolling**: Animated navigation between sections
- **Portfolio Filtering**: Filter projects by category
- **Contact Modal**: Popup contact information
- **Form Validation**: Basic form validation for contact form
- **Scroll Animations**: Elements animate in as you scroll
- **Progress Bar**: Visual scroll progress indicator

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Internet Explorer 11+ (with some limitations)

## 📧 Contact Form Setup

The contact form currently shows an alert message. To make it functional:

1. **Backend Integration**: Connect to a backend service (Node.js, PHP, etc.)
2. **Email Service**: Use services like EmailJS, Formspree, or Netlify Forms
3. **Database**: Store submissions in a database

### Example with EmailJS
```javascript
// Add EmailJS integration
emailjs.send("service_id", "template_id", {
    name: name,
    email: email,
    subject: subject,
    message: message
});
```

### Example with Formspree
```html
<form action="https://formspree.io/f/your-form-id" method="POST">
    <!-- form fields -->
</form>
```

## 🚀 GitHub Pages Features

### Automatic Deployment
- **GitHub Actions**: Automatically deploys on every push to main branch
- **Real-time Updates**: Changes appear on your site within 2-5 minutes
- **Version Control**: Track all changes to your portfolio
- **Free Hosting**: No hosting costs for public repositories

### Custom Domain (Optional)
1. Purchase a domain from a domain registrar
2. Go to **Settings** → **Pages** → **Custom domain**
3. Enter your domain name
4. Configure DNS settings as instructed by GitHub

## 📝 Troubleshooting

### Common Issues

**Site not showing up after deployment:**
- Wait 5-10 minutes for initial deployment
- Check GitHub Actions tab for deployment status
- Ensure repository is public (for GitHub Free accounts)

**Changes not appearing:**
- Check if GitHub Actions workflow completed successfully
- Verify you pushed to the main branch
- Clear browser cache

**404 Errors:**
- Ensure `index.html` is in the root directory
- Check file permissions and names
- Verify `.nojekyll` file exists

### Getting Help

- **GitHub Community**: [GitHub Community](https://github.com/orgs/community/discussions)
- **GitHub Support**: [GitHub Support](https://support.github.com/)
- **Documentation**: [GitHub Pages Documentation](https://docs.github.com/en/pages)

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Feel free to submit issues, feature requests, or pull requests to improve this portfolio template.

## 📞 Support

If you need help customizing or setting up your portfolio, feel free to reach out!

---

**Happy Coding! 🎉**

## 🔗 Useful Links

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Pages Quickstart](https://docs.github.com/en/pages/quickstart)
- [GitHub Actions Documentation](https://docs.github.com/en/actions)
- [Static Site Generators](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site#static-site-generators)