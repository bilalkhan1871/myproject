MY PRODUCTS — PERSONAL INVENTORY APP

FILES
- index.html: app interface and product storage
- manifest.json: Home Screen app settings
- sw.js: offline app shell
- icon.svg: app icon

IMPORTANT
Product records and photos are stored in this browser on this device using IndexedDB. They are not sent to a server by this app. The app code must be served from HTTPS for iPhone Home Screen installation and offline service-worker support. Opening index.html directly from Files is useful for testing but is not the full installable/offline setup.

SETUP (EASIEST ROUTE: NETLIFY OR ANOTHER HTTPS HOST)
1. Upload the files inside this folder to a static hosting service that provides an HTTPS website.
2. Open the HTTPS website address in Safari on your iPhone.
3. Add one test product while online, then refresh once so the offline files are cached.
4. Tap Safari's Share button > Add to Home Screen > Add.
5. Open Trendy Gadgets from the Home Screen. Try turning on Airplane Mode and searching the test product.

PRIVACY
GitHub Pages hosts the app code, not your inventory data. The app does not contain analytics, ads, accounts, or remote database calls. Product photos and details are stored locally in Safari's browser storage. Anyone with access to your unlocked phone/browser may be able to use the app. Do not clear Safari website data unless you have exported a backup.

BACKUPS
Tap Export backup to download a JSON file containing the product details and photos. Keep it somewhere safe. Import backup adds products from a backup file; imported products receive new local IDs so they do not overwrite current items.

LIMITATIONS
- Local data is not automatically shared with other devices.
- Browser storage can be removed by iOS or by clearing website data; export backups regularly.
- If the app is opened under a different website address, it will have a separate inventory.
