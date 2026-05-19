# BetterStartPage

A minimalist, high-performance, and privacy-focused browser start page. BetterStartPage is a standalone, single-file application designed to be portable, fast, and fully customizable without any external dependencies.

Live Demonstration: [the-abra.github.io/BetterStartPage](https://the-abra.github.io/BetterStartPage)


<img width="1920" height="1079" alt="image" src="https://github.com/user-attachments/assets/14bb49df-89ca-4124-84dc-12091d1e1f5d" />

---

## Key Features

### Portability and Privacy
- Single File Architecture: The entire application (HTML, CSS, and JavaScript) is contained within a single index.html file.
- Offline-First: All configuration, categories, and uploaded assets are stored locally in the browser using IndexedDB.
- Zero Network Dependencies: Core functionality works entirely offline, with optional network features for weather and live search suggestions.

### Advanced Customization
- Inline CMS: Access context-aware settings for any element (Clock, Search, Shortcuts, Background) by right-clicking directly on it.
- Desktop Transparency: Background logic supports fixed-attachment wallpapers, allowing the browser to appear transparent when matched with your system wallpaper.
- Dual Backgrounds: Set separate uploaded images for Dark and Light modes.
- Auto Day/Night: Automatically toggles themes based on the system clock (6:00 AM to 6:00 PM for Light mode).

### Widgets and Tools
- Quick Notes: A built-in glassmorphic scratchpad for temporary notes, accessible via the UI or the 'n' keyboard shortcut.
- Weather Widget: Real-time local weather powered by the Open-Meteo API, requiring no API keys.
- Live Search: Integrated autocomplete suggestions from DuckDuckGo combined with local category and shortcut matching.
- Service Profiles: Instant presets for common service bundles including Google, Proton, and Social Media profiles.

### Data Management
- Backup and Restore: Export your entire setup—including uploaded background images—to a JSON file for easy transfer between browsers or devices.
- Prefix-Free Shortcuts: Navigate directly to your links or categories by typing their name in the search bar without needing special characters.

## Control Scheme

### Mouse Interactions
- Right-Click: Opens the context-aware CMS for the clicked element.
- Click: Standard interaction (Clock toggles 12h/24h, Icons switch search engines).

### Keyboard Shortcuts
- n: Opens the Quick Notes scratchpad (when no input is focused).
- Ctrl + E: Toggles persistent Edit Mode visuals.
- Shift (Hold): Temporarily shows Edit Mode outlines for discoverability.
- Esc: Closes any open CMS popovers or the Quick Notes widget.
- Shift + 1-4: Momentarily switches the active search engine.

## Installation

1. Download the index.html file.
2. Set the file as your browser's "New Tab" page or home page.
3. Right-click anywhere to begin customization.

## Technical Details

- Storage: IndexedDB (database: hp-data) for settings, shortcuts, and binary file blobs.
- Favicons: Resolved via Google S2 Favicon API for high-resolution, service-specific icons.
- Styling: Modern CSS with glassmorphism effects, hardware-accelerated filters, and responsive design.
