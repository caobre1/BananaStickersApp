# 🍌 My Banana Stickers Collection

A responsive, mobile-friendly static website showcasing a beautiful gallery of banana sticker designs.

## Features

✨ **Responsive Design** - Works perfectly on mobile, tablet, and desktop devices  
🎨 **CSS Grid Layout** - Modern, adaptive gallery that adjusts to screen size  
⚡ **Fast Performance** - Pure HTML, CSS, and JavaScript (no frameworks)  
♿ **Accessible** - HTML5 semantic markup with proper alt text  
🎯 **Clean & Modern** - Minimalist design with smooth hover effects  
📱 **Mobile-First** - Optimized for small screens with progressive enhancement  

## Project Structure

```
BananaStickersApp/
├── index.html           # Main HTML file
├── style.css            # Stylesheet with responsive grid
├── gallery.js           # JavaScript that loads images dynamically
├── images.json          # JSON file listing all banana stickers
├── images/
│   └── stickers/        # Folder for banana sticker images
└── README.md            # This file
```

## How to Add More Banana Sticker Images

The gallery **automatically displays all images** from the `images/stickers/` folder! Just follow these simple steps:

### Step 1: Add Your Image File
1. Save your banana sticker image to the `images/stickers/` folder
2. Recommended image size: 400x400px (square aspect ratio works best)
3. Supported formats: JPG, PNG, or WebP
4. Keep file size under 200KB for optimal performance
5. Use descriptive filenames like: `banana-happy.jpg`, `banana-cool.jpg`

### Step 2: Update images.json
1. Open `images.json` in your text editor
2. Add a new entry to the `"stickers"` array with your image details

### Example
If you add a file named `banana-rainbow.jpg`, add this to `images.json`:

```json
{
  "filename": "banana-rainbow.jpg",
  "title": "Rainbow Fun",
  "description": "A colorful rainbow banana sticker"
}
```

### Complete images.json Example
```json
{
  "stickers": [
    {
      "filename": "banana-1.jpg",
      "title": "Classic Yellow",
      "description": "Classic yellow banana sticker"
    },
    {
      "filename": "banana-rainbow.jpg",
      "title": "Rainbow Fun",
      "description": "A colorful rainbow banana sticker"
    }
  ]
}
```

That's it! The gallery will automatically load and display your new image without editing `index.html`.

## Responsive Breakpoints

- **Mobile (< 480px)**: Single column layout
- **Tablet (768px - 1023px)**: 2 columns  
- **Desktop (1024px+)**: 3 columns in grid

The gallery automatically adapts to any screen size using CSS Grid's `auto-fit` feature.

## GitHub Pages Deployment

### Step 1: Create a GitHub Repository
1. Go to [GitHub](https://github.com) and log in
2. Click the "+" icon and select "New repository"
3. Name it `BananaStickersApp` (or your preferred name)
4. Choose "Public" for visibility
5. Click "Create repository"

### Step 2: Upload Your Project
**Option A: Using Git Command Line**
```bash
git init
git add .
git commit -m "Initial commit - banana stickers gallery"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/BananaStickersApp.git
git push -u origin main
```

**Option B: Using GitHub Web Interface**
1. On your repository page, click "Add file" → "Upload files"
2. Drag and drop your project files (all files at root level)
3. Commit the changes

### Step 3: Enable GitHub Pages
1. Go to your repository settings (⚙️)
2. Scroll down to "Pages" section
3. Under "Build and deployment", set source to "Deploy from a branch"
4. Select `main` branch as the deployment branch
5. Save and wait for the green checkmark

Your site will be live at: `https://YOUR_USERNAME.github.io/BananaStickersApp/`

## Local Development

To view your website locally:
1. Open `index.html` in your web browser
2. Or start a local server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Python 2
   python -m SimpleHTTPServer 8000
   ```
3. Visit `http://localhost:8000` in your browser

## Customization Tips

### Change Colors
Edit the CSS variables in `style.css`:
```css
:root {
    --primary-color: #FFD700;     /* Main yellow */
    --secondary-color: #FFA500;   /* Orange */
    --dark-color: #2c3e50;        /* Dark text */
    --light-color: #ecf0f1;       /* Light text */
}
```

### Adjust Gallery Spacing
Modify the `gap` property in `.gallery-container`:
```css
gap: 2rem;  /* Space between items */
```

### Change Font
Replace the font family in `body`:
```css
font-family: 'Your Font Name', sans-serif;
```

## Browser Compatibility

- Chrome/Edge 88+
- Firefox 85+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance Tips

1. **Optimize Images**
   - Use tools like TinyPNG or ImageOptim
   - Aim for 100-150KB per image

2. **Use WebP Format**
   - Modern format for smaller file sizes
   - Supported in all modern browsers

3. **Lazy Loading**
   - Can be added later with native `loading="lazy"` attribute

## SEO Best Practices

- ✅ Title and meta description included
- ✅ Semantic HTML markup (`<header>`, `<main>`, `<article>`, `<footer>`)
- ✅ Descriptive alt text on all images
- ✅ Mobile-friendly responsive design

## License

Feel free to use and modify this project for your banana sticker collection!

## Need Help?

- Check the HTML/CSS comments in the source files
- Ensure image file names match exactly in `index.html`
- Verify images are in the `images/stickers/` folder
- Clear your browser cache if changes don't appear

---

Happy collecting! 🍌✨
