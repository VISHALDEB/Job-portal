# Job Portal

**A modern job portal web application** that enables employers to post job listings and job seekers to browse, save, and apply—with user authentication and job management features.

---

##  Table of Contents

1. [About the Project](#about-the-project)  
2. [Features](#features)  
3. [Demo](#demo)  
4. [Tech Stack](#tech-stack)  
5. [Getting Started](#getting-started)  
   - [Prerequisites](#prerequisites)  
   - [Installation](#installation)  
   - [Running the App](#running-the-app)  
6. [Project Structure](#project-structure)  
7. [Usage](#usage)  
8. [Contributing](#contributing)  
9. [License](#license)  
10. [Contact](#contact)  
11. [Acknowledgments](#acknowledgments)

---

## About the Project

This job portal platform allows:

- Employers to create, edit, delete, and manage job postings  
- Job seekers to search, save, and apply for jobs  
- Email notifications on successful applications  

It aims to streamline job discovery and application processes for both parties.

---

## Features

- **User Authentication**: Sign up, log in/out securely  
- **Job Posting**: Employers can create, update, delete postings  
- **Job Search**: Filter by keywords, title, or location  
- **Application Management**: Save jobs and view applied jobs  
- **Email Notifications**: Automatic confirmation upon applying  
- Optionally, **admin panel** to track overall job-seeker/employer activity  

---

## Demo

Live (if applicable): [job‑portal‑server‑eight‑lake.vercel.app](job‑portal‑server‑eight‑lake.vercel.app) ([github.com](https://github.com/VISHALDEB/Job-Portal))  

*(Or insert a screenshot or GIF here for visual impact.)*

---

## Tech Stack

- **Frontend**: React + Vite + TailwindCSS  
- **Backend**: Node.js, Express.js  
- **Database**: MongoDB (Mongoose ODM)  
- **Authentication**: Clerk  
- **Deployment**: Vercel (Backend + Frontend)  

---

## Getting Started

### Prerequisites

- Node.js v18+  
- npm or yarn  
- MongoDB Atlas / Local MongoDB  
- Clerk API keys

### Installation

```bash
git clone https://github.com/VISHALDEB/Job-Portal.git
cd Job-Portal

# Client
cd client
npm install

# Server
cd ../server
npm install
```

Create a `.env` file in `/server` with:

```
PORT=5000
MONGO_URI=your_database_connection_string
CLERK_SECRET_KEY=your_clerk_secret_key
CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
```

### Running the App

```bash
# Start server
cd server
npm run dev

# Start client
cd ../client
npm run dev
```

Visit `http://localhost:5173` for frontend and `http://localhost:5000` for backend.

---

## Project Structure

```
Job-Portal/
├── client/                       # Frontend (React + Vite)
│   ├── public/                   # Static files
│   ├── src/                      # React source code
│   │   ├── assets/               # Images, icons, static assets
│   │   ├── components/           # Reusable components (JobCard, Navbar, etc.)
│   │   ├── context/              # Global context (AppContext)
│   │   ├── pages/                # Pages (Home, JobDetails, etc.)
│   │   ├── App.jsx               # Root React component
│   │   └── main.jsx              # Entry point
│   └── package.json
│
├── server/                       # Backend (Node + Express)
│   ├── config/                   # Database & server config
│   ├── controllers/              # Route controllers (jobController, companyController, etc.)
│   ├── middleware/               # Middleware (auth, error handling)
│   ├── models/                   # MongoDB models (Job, Company, User)
│   ├── routes/                   # Express routes (jobRoutes, companyRoutes)
│   ├── server.js                 # Entry point for backend
│   └── package.json
│
├── .gitignore
├── README.md
└── LICENSE (optional)
```

---

## Usage

1. **Sign up / log in** as either employer or job seeker  
2. **Employer**: Create or manage job postings  
3. **Job Seeker**: Browse, save, apply  
4. Receive **email confirmation** post-application

*(Add screenshots or walkthrough if desired.)*

---

## Contributing

Contributions are welcome! Feel free to:

- Fork this repo  
- Create a branch for your feature or fix  
- Submit a pull request

Please ensure code style consistency and documentation for new features.

---

## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## Contact

Created by **Vishal Deb**  
- GitHub: [VISHALDEB](https://github.com/VISHALDEB)  
- Email: *your.email@example.com*

---

## Acknowledgments

- README best practices & templates from GitHub community  
- Inspiration and resources from open-source developers  

