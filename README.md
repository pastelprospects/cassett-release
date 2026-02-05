Overview:
Enable desktop users to download the Electron app via the existing PWA install button (installPwaBtn). Mobile users keep the current PWA installation flow.

Desktop: “Download Desktop App” with platform-specific installers (Windows/macOS/Linux).
Mobile: Existing PWA install.
Detection: Desktop vs mobile; show the right option.
Current state: Install logic lives in js/core/install.js; button shows/hides by PWA support and install status. js/core/electron-download-config.js exists but is not wired into index.html or install.js.
