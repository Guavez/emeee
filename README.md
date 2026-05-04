# EasyMoney - Loan Management System

A comprehensive loan origination and management system for lending operations.

## Project Structure

```
ChaNee Loan New/
├── backend/              # Node.js API server (serves both API and frontend)
│   ├── src/
│   │   ├── routes/      # API endpoints
│   │   ├── middleware/  # Auth & error handling
│   │   ├── db/          # Database connection & migrations
│   │   ├── utils/       # Utility functions
│   │   └── services/    # Business logic
│   └── test/            # Test files
├── web/                  # Frontend application
│   ├── index.html       # Main HTML file
│   ├── app.js           # Frontend JavaScript
│   └── styles.css       # Stylesheets
├── data/                 # SQLite database file
├── uploads/              # User uploaded files
│   ├── selfies/         # Borrower selfie photos
│   ├── valid-ids/       # Valid ID documents
│   └── income-proofs/   # Income proof documents
├── scripts/              # Utility scripts
│   ├── python/          # Python utilities (SQLite)
│   └── node/            # Node.js migration scripts
├── assets/               # Static assets
│   └── qr-codes/        # Payment QR codes
├── docs/                 # Documentation
└── logs/                 # Application logs
```

## Getting Started

### Prerequisites
- Node.js 18+ (for backend)

### Starting the Application

```bash
cd backend
npm install
npm start
```

The application runs on `http://127.0.0.1:3000`

The Node.js backend serves both the API and the frontend static files.

## Default Admin Credentials

Email: `ruzolshanee@gmail.com` or `ninacharish@gmail.com`  
Password: `Chanee@easymoney0308`

**⚠️ Important:** Change these default credentials in production.

## Database

The database uses SQLite and is located at `data/loan_management.db`. The Node.js backend automatically creates and migrates the database on startup.

## Scripts

### Python Scripts (`scripts/python/`)
- `database.py` - Database management utilities (uses SQLite)
- `seed_admins.py` - Seed admin users

### Node.js Scripts (`scripts/node/`)
- `migrate_to_usage_tracking.js` - Database migration script

## Payment QR Codes

Payment QR codes are located in `assets/qr-codes/`:
- credit-card-qr.jpg
- debit-card-qr.jpg
- gcash-qr.jpg
- paymaya-qr.jpg
- paypal-qr.jpg

## Documentation

- `docs/amortization-schedule.pdf` - Loan amortization documentation
- `docs/payment-history.csv` - Payment history template

## Features

- **Borrower Management** - Register and manage borrowers
- **Loan Applications** - Process loan applications
- **Loan Tracking** - Track active loans and payments
- **Document Management** - Upload and review borrower documents
- **Admin Dashboard** - Comprehensive admin interface
- **Accessibility** - WCAG AA compliant design for low vision users

## License

Proprietary - All rights reserved.
