# 📊 Result Viewer DIU

Result Viewer DIU is an open-source result aggregation platform designed for students of **Daffodil International University (DIU)**. The project aims to provide a faster, more reliable way to access academic results, complete with insights, visualizations, and batch-wide result analysis.

## 🚀 Motivation

This project was born out of a real-world issue — the current university result portal often fails to handle high traffic during result releases. As a student of DIU, I built this platform to alleviate the pressure from the main system and help students get their results smoothly and quickly.

In addition to basic result access, the platform will include statistical graphs, difficulty analysis by subject, and batch-wise result comparisons — making it not just a viewer, but a complete result insight tool.


## 🧠 Key Features

- 🔍 Search any student’s result by ID
- 📈 Batch-wise performance insights
- 📊 Charts and graphs to show grade distributions
- 🧑‍🤝‍🧑 View multiple student results at once
- 🧠 Identify the hardest subjects in each batch
- 🔐 Scraper + Backend API to store results
- ☁️ Cloud-hosted for 24/7 availability


## 🖥️ Demo Frontend

A working demo frontend is under private development. Frontend is built with **ReactJS** using modular components and state management hooks.



## 📦 Tech Stack

- **Frontend:** React.js
- **Backend:** Node.js, Express.js
- **Database:** MongoDB
- **Scraper:** Custom-built using Node.js
- **Hosting:** GitHub Actions, Render (or other free cloud services)


## 🛠️ Setup Instructions

1. Clone the repo
git clone [https://github.com/sanwar-hosen/result-viewer-DIU](https://github.com/sanwar-hosen/result-viewer-DIU)

2. Navigate to backend and install dependencies
cd backend
npm install

3. Add `.env` with Mongo URI and other secrets

4. Run server
node server.js


## ✅ To-Do List

### 🧹 Backend Setup & Scraper

- [x] Create Node/Express backend project
- [x] Write student ID generation logic (batch, programId, roll)
- [x] Add scraping script with failure handling + retries
- [x] Store scraped data in MongoDB
- [x] Prevent duplicate inserts for already-scraped students
- [x] Handle API rate limiting and recovery logic
- [ ] Deploy scraper to the cloud with persistent storage
- [ ] Add resume feature to scraper using last failed ID
- [ ] Build robust error handling for scraper crashes

### 🔌 API Development (Search & View)

- [x] Setup Express routes for API
- [ ] Create endpoint to search result by student ID
- [ ] Create endpoint to list all students (paginated)
- [ ] Add filtering by semester, program, etc.
- [ ] Build endpoint to aggregate stats (avg CGPA, top scorers)
- [ ] Secure API routes with rate limiting

### 🎨 Frontend Development

- [x] Build basic UI with React
- [x] Integrate form to input Student ID
- [ ] Connect frontend with API to fetch result
- [ ] Display result in a styled card or table
- [ ] Add charts (CGPA distribution, hardest subjects)
- [ ] Add batch search feature
- [ ] Add loading and error states

### 📈 Advanced Features

- [ ] Graph view for subject-wise grades
- [ ] Highlight batch toppers
- [ ] Subject difficulty comparison chart
- [ ] Add download/export result feature
- [ ] Add result sharing option


## 📎 Public GitHub Repo

🔗 [https://github.com/sanwar-hosen/result-viewer-DIU](https://github.com/sanwar-hosen/result-viewer-DIU)


## 🙌 Contribution

PRs are welcome! If you're from DIU and want to help out or improve the project, feel free to fork and submit a pull request.


## License

This project is licensed under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License.  
[View LICENSE](./LICENSE.md) | [View Full Legal Terms](https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode)

![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)
