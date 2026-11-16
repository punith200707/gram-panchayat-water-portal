# JalaSeva — Digital Water Complaint Portal

A responsive front-end demo for a Gram Panchayat water complaint portal.

## Run
1. Extract the ZIP file.
2. Open `index.html` in a browser, or use VS Code with the Live Server extension.
3. Submit a complaint, copy the generated complaint ID, and use `Track complaint`.
4. Open `Admin` to change complaint status.

## Included pages
- `index.html` — home page and project overview
- `complaint.html` — complaint registration (photo evidence is not accepted)
- `track.html` — complaint status lookup
- `appointment.html` — water testing appointment requests and status lookup
- `admin.html` — demo dashboard, complaint updates and water testing appointment management
- `style.css` — responsive styling
- `app.js` — demo data handling

## Important limitations
This is a front-end classroom prototype. Data is stored in the browser's localStorage, so it is not shared between devices or browsers and may be lost if browser data is cleared. Photo evidence is disabled; residents submit text details only. The admin page has no authentication. For real deployment, connect a PHP/MySQL backend, implement secure admin login, validate uploads server-side, and add access controls and backups.


## Language
Use the **English / ಕನ್ನಡ** switch in the top navigation on any page. Your selection is remembered in the same browser. The interface includes English and Kannada labels and guidance. User-entered complaint descriptions remain as entered.


Added prototype features: complaint status timeline, in-page status update notifications when a complaint is tracked, customer feedback after resolution, and a demo admin login (password: cit123). IMPORTANT: this project still uses browser localStorage. The demo password is client-side and is NOT secure authentication. True customer/admin accounts, cross-device notifications, shared feedback storage and automatic deletion require a PHP/MySQL backend and server-side authentication/cleanup.

## Water testing appointments
Residents can request a water testing visit by selecting a water source, test type, preferred date and time slot. The portal generates a WT appointment ID that can be used to check the request status. The admin dashboard can mark requests as Requested, Confirmed, Completed or Cancelled. This is a browser-local prototype; requests are not shared across devices and no real testing team is dispatched. A PHP/MySQL backend and secure server-side authentication are required for real deployment.
