# Just Kiddin - Portfolio Website

Retro Soviet-inspired portfolio site for showcasing literary works and music.

## Files Included

- `index.html` - Homepage with navigation to all sections
- `fyva.html` - Dedicated page for ФЫВАПРОЛ novel
- `music.html` - Music albums and streaming links
- `writing.html` - Other literary projects
- `style.css` - Complete styling with retro-futuristic aesthetic
- `cover_typewriter_realistic.svg` - Book cover (add to root directory)

## How to Deploy to GitHub Pages

### Option 1: Web Interface (Easiest)

1. Create a new repository on GitHub
   - Go to github.com and create new repo
   - Name it: `yourusername.github.io` (for personal site)
   - Or any name for project site

2. Upload files
   - Click "uploading an existing file"
   - Drag all files (HTML, CSS, SVG)
   - Commit changes

3. Enable GitHub Pages
   - Go to Settings → Pages
   - Source: Deploy from branch
   - Branch: main
   - Folder: / (root)
   - Save

4. Add custom domain (IONOS)
   - In GitHub Pages settings, add your domain
   - In IONOS DNS settings, add:
     ```
     Type: CNAME
     Name: www (or @)
     Value: yourusername.github.io
     ```
   - Wait 10-30 minutes for DNS propagation

### Option 2: Command Line (Git)

```bash
# Initialize git repository
git init
git add .
git commit -m "Initial commit"

# Create repository on GitHub first, then:
git remote add origin https://github.com/yourusername/yourrepo.git
git branch -M main
git push -u origin main

# Enable GitHub Pages in Settings → Pages
```

## Alternative: Cloudflare Pages

1. Sign up at pages.cloudflare.com
2. Connect to GitHub repository
3. Deploy settings:
   - Build command: (leave empty)
   - Output directory: /
4. Add custom domain in Cloudflare dashboard
5. Update IONOS DNS to point to Cloudflare

## Alternative: Netlify

1. Sign up at netlify.com
2. Drag and drop the entire folder
3. Site is live instantly!
4. Add custom domain in Site Settings
5. Update IONOS DNS as instructed

## Customization

### Adding Your Book Cover
- Replace `cover_typewriter_realistic.svg` with your actual cover
- Or update the path in `fyva.html`

### Adding Music Albums
In `music.html`:
1. Replace placeholder album covers
2. Add actual Spotify/Apple Music embed codes
3. Update album titles, descriptions, and links

### Adding Writing Projects
In `writing.html`:
1. Add more `<article class="writing-item">` blocks
2. Update titles, descriptions, and links
3. Add PDFs or external links

### Changing Colors
In `style.css`, update CSS variables:
```css
:root {
    --color-accent: #00ff88;  /* Change accent color */
    --color-bg: #1a1a1a;      /* Change background */
}
```

## Support

The site is fully static HTML/CSS - no build process needed!
Just edit the HTML files to update content.

## Cost

**FREE** with GitHub Pages or Cloudflare Pages
- Unlimited bandwidth
- Custom domain supported
- HTTPS automatic
