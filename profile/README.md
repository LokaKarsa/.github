# LokaKarsa ✨

### Saka Aksara Tumuju Budaya

<p align="center">
  <img src="logo.png" alt="Logo LokaKarsa" width="150"/>
</p>

## 📖 About The Project

**LokaKarsa** (meaning "The People's Intention" in Sanskrit) is a gamified, Duolingo-style learning application dedicated to teaching and preserving the ancient **Javanese script (Aksara Jawa)**. In an era of globalization, unique cultural treasures like Aksara Jawa face the risk of being forgotten. LokaKarsa aims to reverse this trend by making learning **fun, accessible, and engaging** for a new generation of users worldwide.

Born from a passion for the rich heritage centered in places like Surakarta and Yogyakarta, this app transforms a complex writing system into a playful journey of discovery. Our mission is not just to teach a script, but to reignite curiosity and foster a deeper connection to Indonesian culture.

This project was proudly developed for the **GarudaHacks 6.0 Hackathon** under the **"Connecting Culture"** sub-theme, and is designed to be a ready-to-use application.

---

## 🔥 Features

LokaKarsa is built with a user-centric and pedagogically sound approach, incorporating features designed to maximize learning and engagement.

- **Gamified Learning Path:** A beautiful, vertically scrolling map that guides users through structured levels, from basic letters to complex sentences.
- **Dynamic Quiz Engine:** Say goodbye to boring repetition! Every lesson features a dynamic mix of question types to test different skills:
  - **Multiple Choice:** For visual recognition of characters and words.
  - **Aksara Jawa Handwriting Recognition:** Writing Javanese script and directly identified with AI Model.
  <!-- - **Intelligent Feedback Loop:**
  - **Instant Feedback:** Get immediate visual and audio confirmation for every answer, complete with our mascot, "Karsa," who cheers you on!
  - **"Mistakes Review" Loop:** Our secret sauce! The app remembers your mistakes and re-tests you on them at the end of each lesson, ensuring you truly master the concept before moving on. -->
- **Comprehensive Curriculum:** The learning content is carefully structured:
  - **Level 1: The Basics:** Master the 20 foundational letters.
  - **Level 2: The Hand Writing:** Learn to hand writing javanese script.
  <!-- - **Level 3: Consonant Stacking (Pasangan):** Tackle the advanced skill of writing consonant clusters. -->
- **Engagement & Retention Systems:**
  - **Streaks:** Build a daily learning habit and keep your flame alive! 🔥
  - **XP & Leaderboards:** Earn points for every lesson and compete with others on the global leaderboard.
  - **Achievements:** Unlock badges for reaching significant milestones.
  <!-- - **Contextual "Smart Dictionary":** Don't remember a character? Use the info `(i)` icon during a quiz to get a detailed pop-up with everything you need to know, right when you need it. -->

---

## 🏛️ Architecture Overview

LokaKarsa adopts a decoupled service architecture, allowing for scalability and efficient team development. The project consists of three main repositories:

1.  **[LokaKarsa Frontend](https://github.com/LokaKarsa/LokaKarsa-FE)** (React.js):

    - The interactive and responsive user interface, built with **React (JSX)**.
    - Communicates directly with the **LokaKarsa Backend API** for user data, learning progress, and gamification.
    - Also communicates directly with the **LokaKarsa ML Model API** for handwriting recognition functionality.

2.  **[LokaKarsa Backend API](https://github.com/LokaKarsa/LokaKarsa-BE)** (Laravel):

    - The main backend API built with **Laravel**.
    - Manages user data, learning progress status, leaderboards, and Javanese script content.
    - Interacts with a **MySQL** database.
    - Acts as an intermediary for some requests to the **LokaKarsa ML Model API**, or allows the frontend to interact directly depending on the use case.

3.  **[LokaKarsa ML Model API](https://github.com/LokaKarsa/LokaKarsa-Model-API)** (Flask):
    - A separate API built with **Flask** to host the **Machine Learning model**.
    - Responsible for **recognizing handwritten Javanese script on a canvas**.
    - Provides an endpoint that can be consumed by both the frontend and backend.

---

## 🛠️ Tech Stack

Here are the primary technologies used across the LokaKarsa project:

- **Frontend**: [React.js](https://react.dev/) (with JSX)
- **Backend**: [Laravel](https://laravel.com/) (as a REST API)
- **Database**: [MySQL](https://www.mysql.com/)
- **Machine Learning**: [Flask](https://flask.palletsprojects.com/) (for the ML model API)
<!-- - **Deployment**: (Optional: mention platforms like Vercel, Netlify, Heroku, AWS, GCP, etc. if you have a deployment plan) -->

---

## 🚀 Getting Started

To run the LokaKarsa project locally, you will need to set up each of the three components (Frontend, Backend, and ML Model API) separately. Ensure you have the necessary prerequisites installed for each repository.

### Prerequisites

Make sure you have the following installed on your machine:

- **Node.js** & **npm** (for Frontend)
- **Composer** (for Laravel Backend)
- **PHP** (compatible with the project's Laravel version)
- **Python** & **pip** (for ML Model API)
- **MySQL Server** (for Database)

### Installation Guide

Please follow the links to each repository for more detailed installation guides:

1.  **LokaKarsa Backend API**:

    - Visit: [**`LokaKarsa Backend` README**](https://github.com/your_username/lokakarsa-backend)
    - General steps: `git clone`, `composer install`, `.env` setup, `php artisan migrate`, `php artisan serve`.

2.  **LokaKarsa ML Model API**:

    - Visit: [**`LokaKarsa ML Model` README**](https://github.com/your_username/lokakarsa-ml-api)
    - General steps: `git clone`, `pip install -r requirements.txt`, `python app.py` (or `flask run`).

3.  **LokaKarsa Frontend**:
    - Visit: [**`LokaKarsa Frontend` README**](https://github.com/your_username/lokakarsa-frontend)
    - General steps: `git clone`, `npm install`, ensure API endpoint configuration is correct, `npm start`.

---

## ⚙️ Usage

Once all components (Backend API, ML Model API, and Frontend) are running, you can open your browser to the URL specified by the frontend (typically `http://localhost:3000`). Create an account and follow the on-screen instructions to begin mastering Aksara Jawa!

---

## 🤝 Contributing

Contributions are highly valued! We believe that a strong community is key to the success of open-source projects. If you have a suggestion that would make this better, or would like to add a new feature, please follow the guidelines below.

1.  Fork the relevant repository (`lokakarsa-frontend`, `lokakarsa-backend`, or `lokakarsa-ml-api`).
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`).
3.  Make your changes.
4.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
5.  Push to the branch (`git push origin feature/AmazingFeature`).
6.  Open a Pull Request to the corresponding repository.

Don't forget to give the project a star! Thanks again!

---

## 📄 License

This project is distributed under the **MIT License**. See the `LICENSE.md` file in each individual repository for more information.

---

## 🙏 ACKNOWLEDGMENTS

- **GarudaHacks 6.0**: For this incredible opportunity.
- **Duolingo**: As the primary inspiration for the gamified learning experience.
- All cultural experts and communities dedicated to preserving Aksara Jawa.
