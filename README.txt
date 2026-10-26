MY PRODUCTS — PERSONAL INVENTORY APP

FILES
- index.html: app interface and product storage
- manifest.json: Home Screen app settings
- sw.js: offline app shell
- icon.svg: app icon

IMPORTANT
Product records and photos are stored in this browser on this device using IndexedDB. They are not sent to a server by this app. The app code must be served from HTTPS for iPhone Home Screen installation and offline service-worker support. Opening index.html directly from Files is useful for testing but is not the full installable/offline setup.

SETUP (EASIEST ROUTE: GITHUB PAGES)
1. On a computer, sign in to GitHub and create a new repository, e.g. my-products.
2. Upload all four files from this folder to the repository's root (not the ZIP itself).
3. In the repository, open Settings > Pages.
4. Under Build and deployment, select Deploy from a branch, choose the main branch and /(root), then Save.
5. Wait until GitHub Pages gives you an HTTPS website address.
6. On iPhone, open that HTTPS address in Safari. Add one test product while online, then refresh once so the offline files are cached.
7. Tap Safari's Share button > Add to Home Screen > Add.
8. Open My Products from the Home Screen. Try turning on Airplane Mode and searching the test product.

PRIVACY
GitHub Pages hosts the app code, not your inventory data. The app does not contain analytics, ads, accounts, or remote database calls. Product photos and details are stored locally in Safari's browser storage. Anyone with access to your unlocked phone/browser may be able to use the app. Do not clear Safari website data unless you have exported a backup.

BACKUPS
Tap Export backup to download a JSON file containing the product details and photos. Keep it somewhere safe. Import backup adds products from a backup file; imported products receive new local IDs so they do not overwrite current items.

LIMITATIONS
- Local data is not automatically shared with other devices.
- Browser storage can be removed by iOS or by clearing website data; export backups regularly.
- If the app is opened under a different website address, it will have a separate inventory.
