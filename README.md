# 📚 Shiksha Sagar Library - Live Seat Booking System

A premium, real-time, and loophole-free seat booking web application designed for **Shiksha Sagar Library (Ocean of Learning)**. Built using a serverless architecture to ensure fair seat allocation on a **First-Come, First-Served** basis with zero data redundancy.

🚀 **Live Link:** [ssl-livid.vercel.app](https://ssl-livid.vercel.app)

---

## ✨ Key Features

*   **🔒 Anti-Cheat Google Authentication:** Mandates Google Sign-In to ensure one student gets exactly one chance to book a seat, preventing multiple submissions or script-based spamming.
*   **⚡ Real-Time Live Sync (`onSnapshot`):** Dynamically updates seat availability instantly across all connected client browsers without requiring a page refresh. Taken seats turn red and unclickable in milliseconds.
*   **⚔️ Anti-Clash isolated Transactions (`runTransaction`):** Implements strict database-level operations. If two students attempt to lock the same seat simultaneously, the database serializes the request, granting it to the absolute first millisecond and safely rejecting the overlap.
*   **🎨 Premium Cyber-Ocean Aesthetic:** Styled with premium dark mode gradients using Tailwind CSS, featuring continuous backdrop blur filters and native UI animations for high visual appeal.
*   **🛡️ Secure Production Pipeline:** Designed with zero hardcoded credentials on public source control. Real Firebase API credentials are automatically injected inside Vercel's isolated build wrapper via custom build scripts.

---

## 🛠️ Tech Stack

*   **Frontend:** HTML5, Tailwind CSS (via Play CDN), Vanilla JavaScript (ES6 Modules)
*   **Backend & Database:** Firebase v10 (Authentication & Cloud Firestore)
*   **Hosting & CI/CD:** Vercel integrated via GitHub actions

---

## ⚙️ Project Architecture & Setup

### Dynamic Seat Selection Range
The platform maps available configuration layout natively:
*   **Seats 1 - 10:** Configured exclusively for internal/developer testing purposes.
*   **Seats 39 - 73:** Configured as the real-time active zones for library students.

