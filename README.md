# 🚀 Premium Invoice Generator with Razorpay Integration

A modern, high-performance invoice management system with automated payment collection, professional email delivery, and a sleek dashboard.

## ✨ Key Features

- **💳 Automated Razorpay Payments:** Integrated Razorpay Checkout. Clients can pay via UPI (GPay, PhonePe, Paytm), Cards, or Netbanking.
- **🔄 Smart Status Flow:** 
    - `Draft`: When an invoice is created.
    - `Unpaid`: Automatically changes when the invoice email is sent.
    - `Paid`: Automatically updates the second the payment is captured via Webhooks.
- **📧 Professional HTML Emails:** Beautifully designed emails with billing month details, bold dates, and a "Pay Now" button for clients.
- **⚡ Background Processing:** Emails are sent in the background to ensure the UI stays fast and snappy.
- **📊 Advanced Dashboard:** Real-time stats for Revenue, Pending Payments, and Active Clients with Quick Action buttons.
- **📜 Payment History:** Detailed logs of every transaction including Payer Name, Bank Details, and Transaction IDs.
- **🗑️ Full Management:** Create, Edit, View, and Delete invoices with safety confirmations.

## 🛠️ Technology Stack

- **Frontend:** React.js, Tailwind CSS, Lucide Icons.
- **Backend:** Node.js, Express, MongoDB.
- **Payments:** Razorpay Node SDK.
- **Documents:** PDFKit for professional invoice generation.
- **Mail:** Nodemailer with HTML templates.

## ⚙️ Setup & Installation

### 1. Environment Configuration
Create a `.env` file in the `backend` folder:
```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key

# Email Settings
SMTP_HOST=smtp.gmail.com
SMTP_PORT=465
SMTP_USER=your_email@gmail.com
SMTP_PASS=your_app_password

# Razorpay Keys
RAZORPAY_KEY_ID=rzp_test_...
RAZORPAY_KEY_SECRET=...
RAZORPAY_WEBHOOK_SECRET=your_secret
```

### 2. Install Dependencies
```bash
# In frontend folder
npm install

# In backend folder
npm install
```

### 3. Run the App
```bash
# Start Backend
cd backend
npm start

# Start Frontend
cd frontend
npm run dev
```

## 📈 Future Roadmap
- [ ] Multi-currency support.
- [ ] Recurring subscription billing.
- [ ] Export payment reports to Excel/CSV.

