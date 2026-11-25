# hospital-web
# Al-Zahara Hospital Website

A responsive, single-page hospital website concept for Al-Zahara Hospital in Udayagiri, Mysuru. It combines a public-facing hospital directory and appointment request form with browser-based administration, staff attendance, and appointment management screens.

## Features

- Responsive navigation and hospital overview
- Medical speciality cards and searchable, filterable doctor directory
- Appointment request form with client-side validation and date selection
- Campus location with Google Maps embed, map/satellite/street view controls, and address copy action
- Admin dashboard for editing contact details, doctors, and specialities
- Staff portal for attendance, doctor schedule lookup, and appointment status management
- Persistent demo data using the browser's `localStorage`

## Built with

- HTML5
- Vanilla JavaScript
- Tailwind CSS via its CDN
- Google Fonts (Inter and Plus Jakarta Sans)
- Google Maps embed

There is no package manager, build step, server-side application, or database in this version.

## Run locally

1. Put the HTML file in a folder and rename it to `index.html` (or keep its current name and open that file directly).
2. Keep `image_4f2069.jpg` beside the HTML file to show the hospital campus photo. If it is missing, the page uses an online placeholder image.
3. Open the HTML file in a modern browser. An internet connection is needed for Tailwind CSS, Google Fonts, the map, and the placeholder image.

You can also publish the folder as a static site with GitHub Pages. Set the published source to the branch/folder containing the HTML file and image. If the HTML file is not named `index.html`, link to its filename as the site URL path.

## Demo behavior and limitations

This is a front-end prototype. Appointment requests, doctor/speciality edits, staff accounts, attendance, and session state are saved only in the current browser's `localStorage`. They are not sent to hospital staff or shared with other visitors or devices. Clearing browser data removes this saved state.

The login screens are not secure authentication. The master admin credentials are hard-coded in the JavaScript, and staff account passwords are stored in browser storage. **Do not publish this file with real credentials or use it to handle real patient information.** Before using the site in production, replace the demo login and local storage with a secure server-side authentication system, database, and protected appointment submission flow. Remove any demo credentials and sample patient records before making the repository public.

The HTML contains default hospital contact/location text in more than one place. Review and verify the address, phone numbers, email, opening hours, doctor profiles, specialities, and map location before publishing; update the relevant defaults in the HTML so they are consistent.

## Repository contents

```text
.
├── index.html             # Rename updated2.html to this for standard static hosting
└── image_4f2069.jpg       # Optional campus image referenced by the page
```

If you keep the original filename, replace `index.html` in the tree above with `updated2.html`.

## License

No license is specified. Add a `LICENSE` file before granting others permission to reuse or modify this project.
