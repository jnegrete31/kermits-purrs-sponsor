# Kermit's Purrs - Sponsor Configuration

This repository hosts the remote sponsor configuration for the Kermit's Purrs iOS app. Update the sponsor logo and information here without needing to release a new app version.

## 📁 Repository Structure

```
sponsor/
  ├── config.json    # Sponsor configuration file
  └── logo.png       # Sponsor logo image
```

## 🔧 How to Update Sponsor Information

### Update the Configuration

Edit `sponsor/config.json` with your sponsor details:

```json
{
  "enabled": true,
  "logoUrl": "https://jnegrete31.github.io/kermits-purrs-sponsor/sponsor/logo.png",
  "brandName": "Catfé",
  "url": "https://www.catfe.la"
}
```

**Configuration Options:**
- `enabled`: Set to `true` to show sponsor, `false` to hide it
- `logoUrl`: Direct URL to the logo image (use GitHub Pages URL format)
- `brandName`: Brand name (used as fallback if logo fails to load)
- `url`: Website URL that opens when users tap the sponsor logo

### Update the Logo

1. Replace `sponsor/logo.png` with your new logo
2. Update the `logoUrl` in `config.json` to match (if filename changes)
3. Commit and push to GitHub

**Logo Recommendations:**
- Format: PNG (with transparency) or JPG
- Size: 200-400px width
- File size: Under 500KB for fast loading
- Background: Transparent or white works best

## 🌐 GitHub Pages URLs

After enabling GitHub Pages in your repository settings, your files will be available at:

- **Config:** `https://jnegrete31.github.io/kermits-purrs-sponsor/sponsor/config.json`
- **Logo:** `https://jnegrete31.github.io/kermits-purrs-sponsor/sponsor/logo.png`

## ⚡ How It Works

1. The app checks this repository for the latest sponsor configuration
2. It downloads the logo image from the specified URL
3. Changes appear in the app within 24 hours (or immediately after app reinstall)

## 🚀 Quick Updates

**To change the sponsor logo:**
1. Upload new `logo.png` to `sponsor/` folder
2. Commit and push

**To change sponsor info:**
1. Edit `sponsor/config.json`
2. Commit and push

**To disable sponsor:**
1. Set `"enabled": false` in `config.json`
2. Commit and push

## 📝 Notes

- The app caches the configuration for 24 hours to reduce server load
- If the remote logo fails to load, the app falls back to a local asset or brand name text
- Make sure your repository is **public** for GitHub Pages to work
- Changes may take a few minutes to appear on GitHub Pages after pushing

## 🔗 Links

- **App Repository:** [Kermit's Purrs App](https://github.com/your-username/kermits-purrs)
- **Sponsor Website:** [Catfé](https://www.catfe.la)

