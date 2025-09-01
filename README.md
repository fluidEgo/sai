
# SAI Talent Assessment App

**Smart India Hackathon (SIH) 2025 - Sports Authority of India (SAI) Problem Statement**

The **SAI Talent Assessment App** is a Progressive Web App (PWA) designed to democratize sports talent identification across India, particularly for rural athletes. It allows users to record/upload fitness test videos (e.g., sit-ups, push-ups, vertical jumps, running), analyze them on-device using AI/ML for accuracy and authenticity, and securely submit results to SAI servers. The app features a gamified user interface, performance benchmarking against famous athletes, voice-guided mental games, location-based competition alerts, Aadhaar verification, and certificate parsing, all optimized for low-end smartphones with offline capability.

This project is developed for SIH 2025 using React.js, Flask, Python (MediaPipe, OpenCV), and browser APIs (Web Speech, Geolocation) to meet SAI’s requirements for a low-cost, scalable solution.

## Features
- **Video Upload & Recording**: Record fitness tests via camera or upload videos, using MediaRecorder API.
- **AI/ML Video Analysis**: On-device analysis for sit-ups, push-ups, vertical jumps, and running parameters using MediaPipe and OpenCV, with cheat detection (e.g., tampering, unnatural movements).
- **Secure Data Submission**: Sends user data (profile, metrics, location, certificates) to SAI servers via Flask API with HTTPS.
- **Gamified UI**: Badges, leaderboards, and progress bars, benchmarked against famous athletes (e.g., Usain Bolt’s jump height).
- **Auto Test Segmentation**: Automatically detects and counts exercise reps (e.g., sit-ups, strides).
- **Voice Instructions & Mental Games**: Web Speech API guides users (e.g., “Do 10 sit-ups”) and tests mental focus via voice responses.
- **Location-Based News**: Geolocation API detects user location; Web Push API sends nearby competition alerts.
- **Aadhaar Verification**: Secure eKYC integration for user authentication (mock implementation per UIDAI guidelines).
- **Certificate Parsing**: OCR (Tesseract.js) extracts parameters (e.g., height) from uploaded certificates.
- **PWA**: Offline access, installable on Android/iOS, optimized for low-bandwidth rural areas.
- **Officials’ Dashboard**: Web interface for SAI officials to view athlete data with filters (e.g., by gender).

## Technologies Used
- **Frontend**: React.js (via CDN), Tailwind CSS, Axios, Tesseract.js (OCR), Web Speech API, Geolocation API, MediaRecorder API.
- **Backend**: Flask, SQLite, Flask-CORS.
- **AI/ML**: Python, MediaPipe, OpenCV, NumPy, Pyodide (browser-based Python).
- **PWA**: Service Worker, Web Manifest.
- **Deployment**: Vercel (frontend), Render (backend).

## Prerequisites
- **Node.js**: For running the frontend (`http-server`).
- **Python 3**: For backend and AI/ML.
- **Git**: For cloning the repository.
- **Browser**: Chrome or Firefox (for PWA testing).
- **Mobile Device**: For testing PWA installation and camera features.

## Usage
1. **Athlete Interface** (`index.html`):
   - Open the app in a browser or install as a PWA.
   - Enter profile details (name, age, gender, Aadhaar number).
   - Record/upload a fitness test video (e.g., sit-ups).
   - Click “Analyze Video” to get AI-based metrics (e.g., sit-up count, jump height).
   - View badges (e.g., for beating benchmarks) and leaderboard.
   - Submit data to SAI servers securely.
   - Use voice instructions for guidance (e.g., “Do 10 push-ups”).
   - Play mental focus games via voice responses.
   - Receive alerts for nearby competitions (mock data).

2. **Officials’ Dashboard** (`dashboard.html`):
   - Access `http://localhost:8080/dashboard.html`.
   - View athlete data (name, metrics) in a table with filters (e.g., by gender).
   - Secure login (mock implementation).

3. **Offline Mode**:
   - Record/analyze videos offline (AI runs via Pyodide).
   - Data syncs to SAI servers when online.

## Team Roles and Contributions

## Demo

## Learning Resources
- **React.js**: “React JS Crash Course” (Traversy Media, YouTube).
- **Flask**: “Flask Tutorial for Beginners” (Tech With Tim, YouTube).
- **AI/ML**: “MediaPipe Pose Detection” (Google Developer Blog), “Workouts Monitoring using Ultralytics YOLOv8” (YouTube).
- **PWA**: “Progressive Web App Tutorial” (freeCodeCamp).
- **Voice & Geolocation**: “Web Speech API Tutorial” (Web Dev Simplified), “PWA Geolocation Push Notifications” (Google Developers).
- **OCR & Aadhaar**: “Tesseract.js OCR Tutorial” (YouTube), UIDAI Developer Section.

## Acknowledgments
- **SIH 2025**: For the opportunity to solve real-world problems.
- **Open-Source Tools**: React, Flask, MediaPipe, OpenCV, Pyodide, Tesseract.js.
- **Team**: Six dedicated freshers building a solution for Indian sports talent.

## License
---

