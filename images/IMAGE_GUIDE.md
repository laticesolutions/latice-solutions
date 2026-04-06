# Images Folder - Asset Guide

This folder contains all visual assets for the Latice Solutions website.

## 📁 Current Files

- `favicon.svg` - Website icon (displayed in browser tab)

## 🎨 Recommended Images to Add

### 1. Company Logo
- **File name:** `logo.svg` or `logo.png`
- **Size:** 200x200px minimum
- **Format:** SVG preferred (scales perfectly), or PNG with transparent background
- **Usage:** Navigation bar, footer
- **Design:** Should match your brand identity

### 2. Hero Background (Optional)
- **File name:** `hero-bg.jpg` or `hero-bg.webp`
- **Size:** 1920x1080px
- **Format:** WebP (best compression) or JPG
- **Design:** Subtle, abstract, tech-themed
- **Purpose:** Background for hero section (currently uses CSS gradient)

### 3. Product Icons/Images
- **File names:** 
  - `telcodoc-icon.png` (TelcoDoc AI)
  - `netconfig-icon.png` (NetConfig AI)
  - `telcoops-icon.png` (TelcoOps Agent)
- **Size:** 400x400px
- **Format:** PNG with transparency or WebP
- **Design:** Clean, modern, represents each product

### 4. Screenshots/Mockups (Optional)
- **File names:** 
  - `telcodoc-screenshot.png`
  - `netconfig-dashboard.png`
  - `telcoops-interface.png`
- **Size:** 1200x800px
- **Format:** WebP or PNG
- **Purpose:** Product detail views, demos

### 5. Team Photos (Optional)
- **File names:** `team-member-1.jpg`, etc.
- **Size:** 400x400px (square)
- **Format:** JPG or WebP
- **Purpose:** About/Team section (not currently in design)

## 🛠️ How to Optimize Images

### Before Uploading:

1. **Resize** to recommended dimensions (don't upload 4K images)
2. **Compress** using:
   - Online: https://squoosh.app
   - Mac: ImageOptim (free app)
   - Command line: `cwebp image.jpg -q 80 -o image.webp`
3. **Convert to WebP** for best compression (60-80% smaller than JPG)

### Image Optimization Tools:

- **Squoosh** (Web): https://squoosh.app
- **TinyPNG** (Web): https://tinypng.com
- **ImageOptim** (Mac): https://imageoptim.com
- **RIOT** (Windows): Free image optimizer

## 📝 Using Images in HTML

### Logo in Navigation:
```html
<a href="#home" class="nav-logo">
    <img src="images/logo.svg" alt="Latice Solutions" width="32" height="32">
    <span>Latice Solutions</span>
</a>
```

### Product Icons:
```html
<div class="product-icon">
    <img src="images/telcodoc-icon.png" alt="TelcoDoc AI">
</div>
```

### Hero Background:
```html
<!-- In index.html, replace hero-background div -->
<div class="hero-background" style="background-image: url('images/hero-bg.jpg');"></div>
```

### CSS Background:
```css
.hero-background {
    background-image: url('../images/hero-bg.jpg');
    background-size: cover;
    background-position: center;
}
```

## ✅ Image Checklist

For production-ready site:

- [ ] Company logo added
- [ ] Favicon updated (or keep provided one)
- [ ] Product icons/screenshots added
- [ ] All images compressed
- [ ] WebP format used where possible
- [ ] Alt text added for accessibility
- [ ] Images optimized for mobile (responsive)

## 🎨 Design Tips

1. **Consistency**: Use same style for all product icons
2. **Brand Colors**: Match your color scheme (#007AFF by default)
3. **Quality**: High resolution, but optimized file size
4. **Accessibility**: Always include descriptive alt text
5. **Format**: SVG for logos/icons, WebP for photos

## 📐 Image Dimensions Reference

| Image Type | Recommended Size | Max File Size |
|------------|-----------------|---------------|
| Logo | 200x200px | <50KB |
| Favicon | 32x32px | <10KB |
| Hero Background | 1920x1080px | <200KB |
| Product Icons | 400x400px | <100KB |
| Screenshots | 1200x800px | <200KB |
| Thumbnails | 300x200px | <50KB |

## 🌐 Placeholder Service (Temporary)

While creating your images, use placeholders:

- **Lorem Picsum**: `https://picsum.photos/400/400`
- **Placeholder.com**: `https://via.placeholder.com/400x400`
- **IconScout**: Free icons https://iconscout.com

Example:
```html
<img src="https://via.placeholder.com/400x400/007AFF/FFFFFF?text=TelcoDoc+AI" alt="TelcoDoc AI">
```

---

**Note:** The website works perfectly without custom images (uses emoji icons and CSS gradients). Add images when ready to enhance visual appeal.
