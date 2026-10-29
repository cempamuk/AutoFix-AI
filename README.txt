AUTOFIX AI — FIRST WORKING PROTOTYPE

WHAT WORKS
- VIN entry and VIN decoding via NHTSA vPIC public API (internet required)
- Camera capture + OCR attempt using Tesseract.js CDN (HTTPS and internet required; always verify the VIN)
- Manual vehicle details
- Built-in lookup for a starter set of common OBD-II codes
- Symptom-based troubleshooting checklists
- General repair checklists for cooling, oil leaks, brakes, suspension, battery/starting and misfires
- Locally stored parts notebook and maintenance reminders
- JSON export of saved vehicle/parts/maintenance data
- PWA manifest and service worker for home-screen installation/offline shell

IMPORTANT LIMITATIONS
This is a prototype, not a certified diagnostic tool. It does not connect to the vehicle ECU; live data requires a compatible OBD-II adapter and additional integration. VIN decode may not provide exact trim/options. The repair checklists are general and intentionally do not invent vehicle-specific torque specs. Confirm factory service information, fluids, fitment, recalls and procedures for the exact vehicle. Brakes, steering, suspension and cooling-system work can be safety-critical.

HOW TO TEST ON IPHONE
1. Upload the contents of this folder to a static HTTPS host (for example GitHub Pages, Netlify or Cloudflare Pages).
2. Open the HTTPS URL in Safari on iPhone.
3. Tap Share > Add to Home Screen.
4. Allow camera access if you want to try OCR VIN capture. Manual VIN entry always remains available.
5. Try decoding a VIN while online. Saved notes are stored in that browser on that device.

To make it a true App Store app later, wrap the web app with a native shell (e.g. Capacitor), add a robust VIN/OCR workflow, test on real devices, and review privacy, safety and app-store requirements.
