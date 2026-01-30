# Digital Cortex Website

This is the official website for the Digital Cortex project - an AI-powered knowledge management system.

## Structure

```
website/
├── index.html          # Main HTML file
├── css/
│   └── style.css      # Stylesheet
├── js/
│   └── main.js        # JavaScript functionality
└── README.md          # This file
```

## Running the Website

### Option 1: Open directly
Simply open `index.html` in your web browser.

### Option 2: Local server (recommended)
For better performance and to avoid CORS issues:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (with http-server)
npx http-server

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## Features

- **Responsive Design**: Works on desktop, tablet, and mobile
- **Smooth Animations**: Scroll-triggered animations and smooth transitions
- **Modern UI**: Clean, professional design with gradient accents
- **Interactive Navigation**: Smooth scrolling between sections
- **Showcase Sections**:
  - Hero section with project introduction
  - About section explaining the project
  - Features showcase
  - System architecture overview
  - Development roadmap
  - Contact/contribution information

## Customization

### Colors
Edit the CSS variables in `css/style.css`:
```css
:root {
    --primary-color: #6366f1;
    --secondary-color: #8b5cf6;
    /* ... other colors */
}
```

### Content
Update the content in `index.html` to match your project details.

### GitHub Links
Replace placeholder GitHub URLs with your actual repository:
- Update links in the Hero section
- Update links in the Contact section

## Technologies Used

- HTML5
- CSS3 (with custom properties)
- Vanilla JavaScript
- Google Fonts (Inter)

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Opera (latest)

## License

This website is part of the Digital Cortex project and follows the same license.
