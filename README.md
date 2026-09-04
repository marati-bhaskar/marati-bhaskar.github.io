# Marati Bhaskar - Personal Website

A clean and professional personal website showcasing my academic profile, research, and achievements.

## 🌐 Live Website

Visit the website at: `https://marati-bhaskar.github.io/`

## 📋 About

This is a personal website for Marati Bhaskar, PhD Scholar in Computer Science & Engineering at IIT Tirupati, specializing in High-Performance Computing. The website features:

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Clean Interface**: Modern and professional UI/UX design
- **Smooth Animations**: Intersection Observer API for fade-in effects
- **Interactive Navigation**: Smooth scrolling and active section highlighting
- **Accessible**: Semantic HTML and ARIA-compliant

## 🚀 Features

- **Opening Section**: Photograph and formal introduction, visible without scrolling
- **Education Timeline**: Visual timeline of educational background
- **Research & Publications**: Academic publications
- **Awards & Skills**: Recognition, technical skills, and languages
- **Contact**: Multiple ways to get in touch

## 🛠️ Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Modern styling with CSS Grid and Flexbox
- **JavaScript (ES6+)**: Interactive features and animations
- **Font Awesome**: Icons for social links and UI elements
- **GitHub Pages**: Free hosting

## 📁 Project Structure

```
website/
├── index.html                  # Main HTML file
├── styles.css                  # CSS styling
├── script.js                   # JavaScript functionality
├── cs24d001-1-980x843.jpg      # Profile photograph (opening section)
└── README.md                   # This file
```

## 🔧 Local Development

To run this website locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/marati-bhaskar/marati-bhaskar.github.io.git
   cd marati-bhaskar.github.io
   ```

2. Open `index.html` in your web browser:
   ```bash
   # On Linux
   xdg-open index.html
   
   # On macOS
   open index.html
   
   # On Windows
   start index.html
   ```

   Or use a local server (recommended):
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Python 2
   python -m SimpleHTTPServer 8000
   
   # Using Node.js (if you have http-server installed)
   npx http-server
   ```

3. Visit `http://localhost:8000` in your browser

## 🚢 Deployment to GitHub Pages

### Initial Setup

1. Create a new repository on GitHub named `marati-bhaskar.github.io` (must match your GitHub username for a user page)

2. Initialize git and push to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Personal website"
   git branch -M main
   git remote add origin https://github.com/marati-bhaskar/marati-bhaskar.github.io.git
   git push -u origin main
   ```

3. Enable GitHub Pages:
   - Go to your repository on GitHub
   - Click on **Settings**
   - Scroll down to **Pages** in the left sidebar
   - Under **Source**, select `main` branch
   - Click **Save**
   - Your site will be published at `https://marati-bhaskar.github.io/`

### Updating the Website

To update your website after making changes:

```bash
git add .
git commit -m "Description of changes"
git push
```

Changes will be live within a few minutes.

## 📝 Customization

To customize this website for your own use:

1. **Personal Information**: Update the contact details in `index.html`:
   - Email address
   - Phone number
   - GitHub username
   - LinkedIn URL

2. **Content Sections**: Modify the content in each section to match your profile:
   - Education
   - Research publications
   - Awards and achievements
   - Skills

3. **Colors and Styling**: Edit `styles.css` to change:
   - Color scheme (CSS variables at the top of the file)
   - Fonts
   - Layout and spacing

4. **Functionality**: Modify `script.js` to add or remove features:
   - Navigation behavior
   - Animations
   - Interactive elements

## 🎨 Color Scheme

The website uses the following primary colors (defined in CSS variables):

- Primary: `#1c2733` (Ink)
- Secondary: `#34556e` (Muted slate blue)
- Accent: `#24394b` (Deep slate)
- Text: `#3b4551` (Body text)
- Background: `#f6f7f8` (Light neutral)
- Rules and borders: `#e4e7ea` (Hairline grey)

## 📱 Responsive Breakpoints

- Desktop: > 768px
- Tablet: 481px - 768px
- Mobile: ≤ 480px

## 🔍 SEO Features

- Semantic HTML5 markup
- Meta description and author tags
- Proper heading hierarchy (H1, H2, H3)
- Alt text for images
- Fast loading times

## 📄 License

This project is open source and available for personal use. Feel free to fork and customize for your own website.

## 📧 Contact

**Marati Bhaskar**
- Email: cs24d001@iittp.ac.in
- GitHub: [@marati-bhaskar](https://github.com/marati-bhaskar)
- LinkedIn: [Marati Bhaskar](https://www.linkedin.com/in/marati-bhaskar-b256841b0/)

---

**Current CGPA**: 9.48/10  
**Research Area**: High-Performance Computing  
**Institution**: Indian Institute of Technology Tirupati

Made with ❤️ using HTML, CSS, and JavaScript

