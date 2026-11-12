# Felovia College — Responsive Website Demo

A modern, responsive front-end starter project for **Felovia College of Arts and Science and Engineering**, built with HTML5, CSS3 and vanilla JavaScript.

## Included
- Premium responsive landing page and mobile navigation
- About, programmes, campus life, events, gallery and faculty sections
- Course search and category filtering
- Dark/light theme preference saved in local storage
- Admissions enquiry form with client-side validation
- Demo student/staff login modal
- Keyword-based assistant widget (not an AI chatbot)
- Gallery lightbox
- Scroll reveal animations and reduced-motion support
- PWA manifest and service worker starter
- Local browser storage for demo theme and enquiry submissions

## Run locally
1. Extract the ZIP.
2. Open a terminal in this folder.
3. Run a local static server, for example:
   - `python -m http.server 8000`
   - or use the VS Code Live Server extension.
4. Visit `http://localhost:8000`.

A local server is recommended for service-worker/PWA testing. Google Fonts and Unsplash images require an internet connection.

## Important: demo versus production
This is a complete **front-end demonstration**, not a production-ready college management backend. The login does not authenticate users. Enquiry data is stored only in the visitor's browser and is not sent to the college. The assistant uses simple keyword matching and is not connected to an AI model. Student attendance, marks, fee payments, staff records, admissions workflows and administrator controls need a secure server and database.

Before launch:
- Verify the official college name, approved programmes, faculty profiles, contact details, campus address, events, images and admission dates.
- Add a backend API and database (for example, Node.js/Express with PostgreSQL or MySQL).
- Implement secure authentication, role-based permissions, password hashing, session management, CSRF protection, rate limiting, audit logs and backups.
- Validate all data on the server; do not rely on browser validation or localStorage for sensitive data.
- Add a privacy notice, consent language, retention policy and secure contact/enquiry handling.
- Replace placeholder/demo content and test accessibility, mobile layouts, performance and security.

## Suggested full-system modules
1. Public website and CMS
2. Admissions: enquiry, application, document upload, review and status tracking
3. Student portal: profile, timetable, attendance, results and notices
4. Faculty portal: class lists, attendance entry, internal marks and resources
5. Admin dashboard: role-based user management, courses, departments, events and reports
6. Notifications: email/SMS/push via trusted providers
7. Finance: fee invoices and payment gateway integration (never store card data yourself)

## Project structure
- `index.html` — page structure and sections
- `styles.css` — responsive design system and components
- `app.js` — UI interactions and demo behaviour
- `manifest.webmanifest` — PWA metadata
- `service-worker.js` — basic static asset caching


## College branding assets
- `assets/felovia-crest.png` — supplied crest used in the header and footer.
- `assets/favicon-64.png` — browser tab favicon.
- `assets/favicon-192.png` and `assets/favicon-512.png` — PWA/app icons.


## Student portal preview (added)
- Student demo profile registration and register-ID sign-in (no password storage)
- Student dashboard and profile with digital ID preview
- Attendance summary and subject-wise attendance
- Internal assessment marks and semester result preview
- Assignment file selection preview and study-material placeholders
- Weekly timetable and local leave-request form
- Fee history preview and fee-statement request (no payment processing)
- Bonafide and transfer-certificate request forms
- Sample academic calendar and student notifications
- Demo requests saved in browser localStorage

**Production requirements:** This portal is a front-end prototype. Browser storage is not a secure student database. Before deployment, implement server-side identity verification, role-based access, encrypted transport, secure database storage, file scanning/access controls, audit trails, official data integrations, and a compliant payment gateway. Do not use the sample marks, attendance, fee entries or calendar as real college information.


## Admin dashboard preview (added)
- Super-admin sign-in screen and admin workspace navigation
- Dashboard KPI cards and operational analytics snapshot
- Student, faculty, department and course record management
- Admission application tracking and status fields
- Attendance monitoring records
- Examination schedule management
- Fee record management (no payment collection)
- Notice publishing status management
- User role and permission-label management
- Website page/section content status management
- CSV exports for module reports and audit activity
- Local activity log for create, update, delete and export actions
- Demo records persist in browser localStorage

**Security / production note:** The sign-in form is intentionally a visual prototype and accepts non-empty credentials; it is not real authentication. Browser localStorage and client-side role labels are not secure. Production deployment requires server-side authentication (preferably MFA), role-based authorization enforced by the API, secure database access, CSRF/XSS protections, encrypted transport, validated uploads, payment-provider integration, immutable server-side audit logs, backups and tested access controls. All included records and analytics are illustrative only.

## Faculty Portal (demo)
The Faculty Portal is available from the main navigation. Faculty can create a browser-local demo profile and explore profile details, class management, attendance entry, marks upload, assignment creation/evaluation, study materials, timetable, performance reports, leave requests, salary information guidance, and internal communication. Demo records are stored in the current browser using localStorage. This is a front-end prototype only; production use requires secure server-side authentication, role-based permissions, validated academic data, protected file storage, and an authorised HR/payroll integration.
