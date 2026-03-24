# SiinQee Lease Management System

A modern, full‑featured lease management platform designed for capital goods financing. This system supports multiple user roles (Client, Vendor, Branch Staff, CRMD, Admin) and manages the entire lease lifecycle – from application submission and document verification to payment scheduling and asset tracking.

## 🚀 Features

### 🔐 Multi‑Role Authentication & Dashboards
- **Client Dashboard**: Track application status, view payment schedules, upload documents, request branch transfers.
- **Vendor Dashboard**: List products, manage inventory, view applications.
- **Branch Staff Dashboard**: Review assigned applications, forward to CRMD, schedule site visits.
- **CRMD Dashboard**: Oversee all applications, manage document verification, approve transfers.
- **Admin Dashboard**: Full user and system management, report generation, product approval.

### 📝 Application Workflow
- Multi‑step application form (Personal, Business, Equipment details)
- Sector‑based down payment & service charge calculations (from tariff document)
- Product catalog with manual entry option
- Branch assignment based on zone/town
- 8‑stage progress tracking with visual bar

### 📄 Document Management
- Required document checklist per stage
- Upload documents (TIN, licenses, bank statements, etc.)
- Admin/CRMD verification
- File storage with links in database

### 💰 Payment & Financial
- Automatic payment schedule generation
- Installment editing (admin)
- Late payment penalty calculation (2% per month)
- PDF export of payment schedule

### 🔔 Notifications
- In‑app notifications for status changes
- Email/SMS queue (ready for integration)
- 3‑day pending application reminder (cron job)

### 🛠️ Additional Tools
- Branch management (with manager assignment)
- User management (approve, reject, edit roles)
- Product management (vendor submissions, admin approval)
- Branch transfer requests (client/branch initiated)
- Lease calculator for main website

## 🧰 Technologies Used

- **Backend**: PHP 8.1+, SQLite3
- **Frontend**: Tailwind CSS, Font Awesome, JavaScript (ES6)
- **Database**: SQLite (single file, no separate server)
- **Authentication**: Session‑based with password_hash()
- **PDF Generation**: mPDF (optional, fallback HTML)

## 📦 Installation

### Prerequisites
- PHP 8.1 or higher with SQLite3 extension enabled
- Web server (Apache/Nginx)
- Composer (optional, for mPDF)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/lease_management.git
   cd lease_management
