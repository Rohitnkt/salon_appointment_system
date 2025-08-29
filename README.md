# Salon Appointment Management System

A full-stack web application for booking, managing, and tracking salon appointments.

## Features

### User Side

- Book appointments with name, email, phone, date, time, and service
- Receive confirmation or rejection emails

### Admin Side

- Secure admin login (credentials stored via environment variables)
- View dashboard with all appointments: pending, confirmed, rejected
- One-click approval/rejection
- Statistics panel showing totals

---

## Tech Stack

| Layer    | Technology                      |
| -------- | ------------------------------- |
| Backend  | Node.js, Express                |
| Database | SQLite                          |
| Frontend | HTML, CSS, JavaScript           |
| Email    | Nodemailer + Gmail App Password |

---

## Screenshots

> All screenshots are stored in the `assets/images/` folder.

### Home Page

![Home Page](assets/images/home-page.png)

### Services Section

![Services](assets/images/services-section.png)

### Booking Form

![Booking Form](assets/images/booking-form.png)

### Admin Login

![Admin Login](assets/images/admin-login.png)

### Admin Dashboard

![Admin Dashboard](assets/images/admin-dashboard.png)

### Email - Booking Message

![Email Booking Message](assets/images/email-bookingmessage.png)

### Email - Confirmation Message

![Email Confirmed](assets/images/email-confirmed.png)

---

## Getting Started

### Prerequisites

- Node.js (v18+)
- Gmail account with App Password enabled

### Installation

```bash
git clone https://github.com/rohitnkt/salon-appointment-system.git
cd salon-appointment-system
npm install
```

### Environment Setup

Create a `.env` file in the root directory:

```env
EMAIL_USER=yourgmail@gmail.com
EMAIL_PASS=yourapppassword
ADMIN_USER=youradminusername
ADMIN_PASS=youradminpassword
```

> ⚠️ Don’t commit your `.env` file. It should be listed in `.gitignore`.

---

### ▶️ Run the Application

```bash
node server.js
```

Then open: [http://localhost:8000](http://localhost:8000)

---

## 📂 Folder Structure

```
salon-appointment-system/
├── client/
│   ├── index.html
│   ├── styles.css
│   └── script.js
├── admin.html
├── admin.js
├── server.js
├── salon.db
├── .env
├── .gitignore
├── README.md
└── assets/
    └── images/
        ├── home-page.png
        ├── services-section.png
        ├── booking-form.png
        ├── admin-login.png
        ├── admin-dashboard.png
        ├── email-bookingmessage.png
        └── email-confirmed.png
```

---

## ✉️ Email Configuration Notes

- Gmail must have **2-Factor Authentication** enabled
- Generate a Gmail **App Password**:  
  👉 [https://myaccount.google.com/apppasswords](https://myaccount.google.com/apppasswords)

---

## 💡 Future Enhancements

- 🔐 JWT-based authentication
- 📱 SMS notifications via Twilio
- 🧾 Appointment summary emails
- 🎨 UI enhancement using TailwindCSS or Bootstrap
- 🌐 Cloud database (e.g., MongoDB, PostgreSQL)

---

## 🤝 Contributing

This is a personal project, but contributions are welcome.  
Feel free to submit issues or pull requests for improvements !

---

## 📄 License

This project is licensed under the [MIT License](LICENSE)
