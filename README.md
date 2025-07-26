
# 🍲 Platr

![Platr Banner](https://www.cleanlink.com/resources/editorial/2024/30746-sstock-2166454163.jpg)

> **Platr** helps businesses reduce food waste and fight hunger by connecting surplus food with those who need it — donors, recipients, and volunteers, all on one platform.

---

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Contributors Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)
![Built With Love](https://img.shields.io/badge/built%20with-%E2%9D%A4-red)

---

## 📚 Table of Contents

- [🌟 Features](#-features)
- [🚀 Getting Started](#-getting-started)
  - [🔧 Prerequisites](#-prerequisites)
  - [⚙️ Installation](#-installation)
- [🛠️ Technology Stack](#️-technology-stack)
- [📁 File Structure](#-file-structure)
- [🌐 API Endpoints](#-api-endpoints)
- [👥 User Roles & Dashboards](#-user-roles--dashboards)
- [🧪 API Documentation](#-api-documentation)
- [☁️ Deployment](#-deployment)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [📬 Contact](#-contact)

---

## 🌟 Features

* **Role-Based Dashboards:** Custom, personalized views for **Donors**, **Recipients**, and **Volunteers** that streamline their specific tasks and workflows.
* **Intuitive Food Listings:** Donors can quickly and easily post details about their surplus food, including quantity, dietary information, and pickup windows.
* **Smart Matching:** The platform intelligently connects food donors with nearby recipient organizations or individuals based on location and specific needs.
* **Real-Time Tracking:** Volunteers can manage their pickup and delivery missions with live updates and integrated mapping to ensure timely and efficient food transfer.
* **In-App Messaging:** A secure communication channel is provided for donors, recipients, and volunteers to coordinate logistics without sharing personal contact information.
* **Impact Reporting:** The system tracks and displays key metrics such as meals provided, food waste diverted from landfills, and the number of lives positively impacted.
* **User Verification:** A robust and thorough vetting process for recipient organizations builds trust and ensures food reaches legitimate non-profits and community groups.

---

## 🚀 Getting Started

Get Platr running locally in 4 easy steps.

### 🔧 Prerequisites

- [Node.js](https://nodejs.org/en/) (v14+)
- [MongoDB](https://www.mongodb.com/try/download/community)
- npm or yarn package manager

### ⚙️ Installation

1.  **Clone the Repo**
    ```bash
    git clone [https://github.com/your-username/Platr.git](https://github.com/your-username/Platr.git)
    cd Platr
    ```

2.  **Install Dependencies**
    ```bash
    # Backend
    npm install

    # Frontend
    cd client
    npm install
    cd ..
    ```

3.  **Environment Setup**
    Create a `.env` file in the root and add:
    ```env
    MONGO_URI=mongodb://localhost:27017/Platr
    JWT_SECRET=your_jwt_secret_key

    CLOUDINARY_CLOUD_NAME=your_cloudinary_name
    CLOUDINARY_API_KEY=your_cloudinary_key
    CLOUDINARY_API_SECRET=your_cloudinary_secret

    MAPBOX_API_KEY=your_mapbox_key
    ```

4.  **Start the App**
    ```bash
    npm run dev        # Backend at http://localhost:5000

    cd client
    npm start          # Frontend at http://localhost:3000
    ```

> Your app should now be running locally! 🎉

---

## 🛠️ Technology Stack

### 🔷 Frontend

* React + React Router
* Tailwind CSS / Material-UI
* Axios for HTTP requests
* Mapbox / Leaflet for maps

### 🔶 Backend

* Node.js + Express
* MongoDB + Mongoose
* JWT + Passport.js
* Cloudinary / Multer for uploads
* Bcrypt for password hashing

---

## 📁 File Structure

```bash
.
├── client/                     # React frontend
│   ├── public/
│   └── src/
│       ├── components/         # UI components
│       ├── hooks/              # Custom logic
│       ├── pages/              # Main views
│       ├── context/            # Global state (auth, user)
│       ├── api/                # Axios calls
│       └── App.js
├── controllers/                # Express logic
├── models/                     # MongoDB schemas
├── routes/                     # API routes
├── middleware/                 # Auth, error handling
├── .env.example
├── package.json
└── server.js                   # Entry point

## 🛠️ Technology Stack

### 🔷 Frontend

* React + React Router
* Tailwind CSS / Material-UI
* Axios for HTTP requests
* Mapbox / Leaflet for maps

### 🔶 Backend

* Node.js + Express
* MongoDB + Mongoose
* JWT + Passport.js
* Cloudinary / Multer for uploads
* Bcrypt for password hashing

---

-----

## 🌐 API Endpoints

| Method | Endpoint                    | Description             | Role      |
| ------ | --------------------------- | ----------------------- | --------- |
| POST   | `/api/auth/register`        | Register user           | Public    |
| POST   | `/api/auth/login`           | Authenticate user       | Public    |
| GET    | `/api/users/profile`        | User profile            | Auth      |
| POST   | `/api/donations`            | Create donation         | Donor     |
| GET    | `/api/donations/donor`      | List donor donations    | Donor     |
| GET    | `/api/donations/available`  | List available food     | Recipient |
| POST   | `/api/requests`             | Request donation        | Recipient |
| GET    | `/api/requests/recipient`   | View recipient requests | Recipient |
| GET    | `/api/deliveries/missions`  | View delivery tasks     | Volunteer |
| PUT    | `/api/deliveries/:id/accept`| Accept task             | Volunteer |
| PUT    | `/api/deliveries/:id/status`| Update delivery status  | Volunteer |

-----

## 👥 User Roles & Dashboards

### 🧑 Donor

  * Post surplus food
  * Track donation impact
  * Message volunteers & recipients

### 🧑‍🦱 Recipient

  * Browse nearby listings
  * Request food
  * Track delivery progress

### 🚴 Volunteer

  * View tasks
  * Accept deliveries
  * Update status in real time

-----

## 🧪 API Documentation

Want to explore the backend API?

> 📘 [View API Reference (Postman Collection)](https://www.postman.com/collections/your-api-link)

Or generate Swagger docs using `swagger-ui-express`.

-----

## ☁️ Deployment

### 🌍 Suggested Platforms

  * **Frontend:** Vercel, Netlify
  * **Backend:** Render, Railway, Heroku
  * **Database:** MongoDB Atlas

### 🔐 Environment Vars for Production

Make sure to configure:

  * MongoDB URI
  * Cloudinary keys
  * Mapbox API key
  * JWT Secret

-----

## 🤝 Contributing

We welcome all contributions\! ✨

```bash
# Fork the repo
git checkout -b feature/your-feature
git commit -m "Add your feature"
git push origin feature/your-feature
```

Then open a **Pull Request** 🙌

-----

## 📄 License

This project is licensed under the **MIT License**.
See the [`LICENSE`](https://www.google.com/search?q=./LICENSE) file for details.

-----

## 📬 Contact

Need help or want to collaborate?

  * 🌐 GitHub: [github.com/AmanBhaskar16/Platr](https://github.com/AmanBhaskar16/Platr)
  * 📧 Email: [amanbhaskar16@gmail.com](mailto:amanbhaskar16@gmail.com)

-----

```
```
