# Cryptic Finds - TechTatva CTF Platform

This repository contains the code for the official Capture the Flag (CTF) platform used for "Cryptic Finds," an event during TechTatva, the annual technical fest of Manipal Institute of Technology.

**My Role:** Team Lead & Full Stack Developer

**Live Link:** [**https://cryptic-finds.vercel.app/**](https://cryptic-finds.vercel.app/)

> **Note:** This is a cleaned, public-facing portfolio version of the original codebase. All sensitive keys, credentials, and event-specific data have been removed.

---

## 🚀 About The Project

Our team was responsible for building a secure, scalable, and real-time platform from scratch to host the CTF event. The platform needed to handle 500+ participants simultaneously, manage challenge submissions, validate flags securely, and display a live leaderboard.




### Key Features

* **Real-time Leaderboard:** A live, auto-updating leaderboard built with Firestore listeners to show participant rankings instantly.
* **Secure Flag Validation:** All flag submissions were handled by serverless functions (Firebase Functions) to prevent client-side exploits and ensure integrity.
* **Scalable Architecture:** Built on a serverless stack (Firebase and Vercel) that automatically scaled to handle peak traffic during the event without any downtime.
* **Full Deployment:** I managed the complete deployment pipeline, including connecting the custom `crypticfinds.site` domain and configuring DNS.
* **Challenge Management:** A RESTful API structure for fetching, managing, and tracking progress on all CTF challenges.

---

## 🛠 Tech Stack

* **Frontend:** React.js, Next.js
* **Backend:** Firebase Functions (Node.js)
* **Database:** Firestore (NoSQL)
* **Authentication:** Firebase Authentication
* **Deployment:** Vercel (Frontend) & Firebase (Backend Functions)

---

## Running The Project Locally

### 1. Prerequisites

You will need to have [Node.js](https://nodejs.org/) and [Git](https://git-scm.com/) installed on your machine.

### 2. Setup

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/YourUsername/techtatva-ctf-platform-portfolio.git](https://github.com/YourUsername/techtatva-ctf-platform-portfolio.git)
    cd techtatva-ctf-platform-portfolio
    ```

2.  **Install dependencies:**
    ```sh
    npm install
    ```

3.  **Set up environment variables:**
    * Create a `.env.local` file in the root of the project.
    * You will need to create your own Firebase project to get these credentials.
    * Copy the structure from `.env.example`:

    ```env
    # .env.example
    # Firebase client-side config
    NEXT_PUBLIC_FIREBASE_API_KEY=YOUR_KEY_HERE
    NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=YOUR_KEY_HERE
    NEXT_PUBLIC_FIREBASE_PROJECT_ID=YOUR_KEY_HERE
    NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=YOUR_KEY_HERE
    NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=YOUR_KEY_HERE
    NEXT_PUBLIC_FIREBASE_APP_ID=YOUR_KEY_HERE
    ```

4.  **Run the development server:**
    ```sh
    npm run dev
    ```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the result.
