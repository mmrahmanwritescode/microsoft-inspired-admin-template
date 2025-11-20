microsoft-inspired-admin-template
=================================

Overview
--------
This repository provides a lightweight, Microsoft-inspired admin dashboard HTML/CSS template designed for quick prototyping and reuse across internal systems. The template focuses on consistent, reusable CSS variables and components (headers, forms, inputs, cards, tables) and uses Bootstrap + Font Awesome for layout and icons.

What is built so far
--------------------
- Consistent design system using CSS variables in `styles.css` (colors, spacing, border colors, sidebar width, etc.).
- Pages (static HTML):
  - `dashboard.html` — Main dashboard with stat cards and recent items table.
  - `product-list.html` — Product listing with search and actions.
  - `product-add.html` — Product add/edit form with icons and input meta descriptions.
  - `user-list.html` — User listing with search and actions.
  - `user-add.html` — User add/edit form modeled after product-add, includes role selection and meta descriptions.
  - `profile-edit.html` — Edit profile page with profile photo section and change password fields.
  - `login.html` — Auth UI with icons and helper text.
  - `register.html` — Registration UI with icons and helper text.
  - `reset-password.html` — Reset password UI with icon header and helper text.

UI/UX Enhancements implemented
-----------------------------
- Page headers include an icon, engaging title and a subtitle.
- Right-aligned contextual action button (e.g., "Back to Products", "Add Product").
- Form fields include label icons and contextual helper text directly beneath inputs (`.form-meta`).
- Reusable `.form-group-wrapper`, `.form-label`, `.form-meta` classes for consistent input styling.
- Auth pages include navigation links with icon animations (`.auth-nav-links`, `.auth-nav-link`).
- Topbar user dropdown (Edit Profile, Settings, Logout) implemented across main pages.
- Reusable CSS variables (defined in `styles.css`) for easy theming across systems.

Key files
---------
- `styles.css` — Core styling and CSS variables; try to reuse the variables in other projects.
- `product-add.html`, `product-list.html` — Examples of the form/list pattern.
- `user-add.html`, `user-list.html` — User-focused pages following the same pattern.
- `profile-edit.html` — Example settings/profile page.

How to use
----------
1. Open any HTML file directly in your browser (double-click) for quick preview.
2. Edit `styles.css` to change colors or spacing using the CSS variables at the top of the file. The variables are designed to be reused across pages.

Developer notes
---------------
- The template uses Bootstrap 5 for layout and Font Awesome for icons (both loaded via CDN in each HTML file).
- Focus styles and input helper text are included to give an accessible and engaging form experience. Consider adding ARIA attributes for more accessibility improvements.
- The pages are static HTML — integrate them into your framework/backend by converting static form actions and client-side navigation into server routes or SPA routing as needed.

Recommended next steps
----------------------
- Add small JS to handle client-side form validation and show success/error states.
- Add a build step (e.g., Sass + autoprefixer) if you plan to grow the CSS.
- Add lightweight unit/page tests or visual regression checks if the template will be used across multiple applications.

License & attribution
---------------------
- This template is a small personal/prototype template. Replace or add a license file if you plan to publish or reuse widely.
- Bootstrap and Font Awesome are used under their respective licenses (CDN usage). Check their docs for commercial use if required.

