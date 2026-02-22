# Vibe TV

A sleek, responsive TV home page for quick access to your favorite streaming apps and services.

**Live Demo:** https://penguinmenac3.github.io/vibe-tv/

## Features

- 🎯 **Quick App Access** - Large, easy-to-click buttons for your favorite apps
- 🎨 **Dark Theme** - Easy on the eyes with a modern dark interface
- 📱 **Responsive Design** - Works seamlessly on any screen size
- ⌨️ **Keyboard Navigation** - Navigate with arrow keys and press Enter to open apps
- 🎬 **Auto-fetched Icons** - App icons are automatically fetched from favicons
- 💾 **Local Storage** - Your app list is saved locally in your browser
- ⚙️ **Easy Customization** - Add, remove, and manage apps from the settings modal

## Usage

### Online
Simply visit https://penguinmenac3.github.io/vibe-tv/ to start using the app immediately.

### Keyboard Controls
- **Arrow Keys** - Navigate between apps
- **Enter** - Open the focused app
- **ESC** - Open settings

### Adding Apps
1. Click the **Settings (ESC)** button in the top right
2. Enter the app name (e.g., "Netflix")
3. Enter the app URL (e.g., "https://www.netflix.com")
4. Click **Add App**
5. Click **Close (ESC)** to return to the home page

### Removing Apps
1. Open settings
2. Find the app in the "Current Apps" list
3. Click the **Remove** button

### Reset to Default
Click **Reset to Default** in the settings to restore only YouTube.

## Local Development

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/penguinmenac3/vibe-tv.git
   cd vibe-tv
   ```

2. Open `index.html` in your browser or serve it locally:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Python 2
   python -m SimpleHTTPServer 8000
   
   # Using Node.js (with http-server)
   npx http-server
   ```

3. Visit `http://localhost:8000` in your browser

## Customization

### Changing Default Apps
Edit the `DEFAULT_APPS` array in `index.html`:
```javascript
const DEFAULT_APPS = [
  { name: 'YouTube', url: 'https://www.youtube.com' },
  { name: 'Netflix', url: 'https://www.netflix.com' }
];
```

### Styling
All styles are in the `<style>` section of `index.html`. The design uses viewport-relative units (vw) for responsive scaling across all screen sizes.

## Browser Support
Works on all modern browsers that support:
- CSS Grid
- Flexbox
- localStorage API
- ES6 JavaScript

## Notes
- Apps are stored in your browser's localStorage and persist across sessions
- App icons are fetched from Google's favicon service
- No backend required - fully client-side application
- Perfect for use on smart TVs and media center PCs

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

