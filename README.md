# 🚀 GenFlex – AI-Powered Educational Assessment Platform

![GenFlex Banner](https://img.shields.io/badge/GenFlex-AI%20Assessment%20Platform-blue?style=for-the-badge)

![React](https://img.shields.io/badge/Frontend-React%2018-blue)
![Node.js](https://img.shields.io/badge/Backend-Node.js-green)
![Express](https://img.shields.io/badge/API-Express.js-lightgrey)
![MongoDB](https://img.shields.io/badge/Database-MongoDB-success)
![Python](https://img.shields.io/badge/AI-Python-yellow)
![PyTorch](https://img.shields.io/badge/ML-PyTorch-red)
![Transformers](https://img.shields.io/badge/NLP-HuggingFace%20Transformers-orange)
![License](https://img.shields.io/badge/License-MIT-purple)
![Status](https://img.shields.io/badge/Status-Active-success)

---

# 📚 Overview

**GenFlex** is a **full-stack AI-powered educational assessment platform** designed to assist educational institutions in **automatically generating, managing, and evaluating examinations** using modern **Artificial Intelligence and Machine Learning models**.

The platform enables instructors to **generate exams directly from lecture materials**, conduct **timed assessments**, and perform **automated evaluation of student responses** including essays, coding problems, and mathematical solutions.

By combining **modern web technologies with advanced NLP models**, GenFlex significantly reduces the manual workload of instructors while maintaining high-quality assessment standards.

---

# 🎯 Project Goals

GenFlex aims to:

* Automate **exam creation from lecture content**
* Provide **AI-based evaluation** of subjective answers
* Support **coding and mathematical assessments**
* Reduce **manual grading effort**
* Improve **assessment scalability in educational institutions**
* Provide **plagiarism detection and feedback systems**

---

# 🏗 System Architecture

GenFlex follows a **three-layer architecture**:

```
                ┌─────────────────────────┐
                │        Frontend         │
                │        React.js         │
                └────────────┬────────────┘
                             │
                             ▼
                ┌─────────────────────────┐
                │        Backend          │
                │     Node.js + Express   │
                └────────────┬────────────┘
                             │
                             ▼
                ┌─────────────────────────┐
                │        AI Layer         │
                │       Python + ML       │
                └────────────┬────────────┘
                             │
                             ▼
                ┌─────────────────────────┐
                │        Database         │
                │        MongoDB          │
                └─────────────────────────┘
```

### Architecture Components

| Layer        | Technology        | Purpose                            |
| ------------ | ----------------- | ---------------------------------- |
| **Frontend** | React.js          | User interface and interactions    |
| **Backend**  | Node.js + Express | API server and application logic   |
| **AI Layer** | Python ML scripts | Question generation and evaluation |
| **Database** | MongoDB           | Data storage                       |

---

# 💻 Technology Stack

## Frontend

| Technology       | Purpose             |
| ---------------- | ------------------- |
| React 18         | UI development      |
| React Router DOM | Client-side routing |
| Chakra UI        | Component library   |
| Emotion          | Styling             |
| Framer Motion    | Animations          |
| Axios            | API requests        |
| Monaco Editor    | Coding exam editor  |
| React Icons      | UI icons            |

---

## Backend

| Technology | Purpose             |
| ---------- | ------------------- |
| Node.js    | JavaScript runtime  |
| Express.js | REST API framework  |
| MongoDB    | Database            |
| Mongoose   | ODM for MongoDB     |
| JWT        | Authentication      |
| bcryptjs   | Password hashing    |
| Multer     | File uploads        |
| PDFKit     | PDF generation      |
| CORS       | Cross-origin access |

---

## AI / Machine Learning Stack

| Library / Model          | Purpose                          |
| ------------------------ | -------------------------------- |
| HuggingFace Transformers | NLP models                       |
| PyTorch                  | Deep learning framework          |
| Sentence Transformers    | Semantic similarity              |
| KeyBERT                  | Keyword extraction               |
| FAISS                    | Vector search                    |
| spaCy                    | NLP processing                   |
| BART                     | Lecture summarization            |
| T5                       | Question generation              |
| DeepSeek (Fine-tuned)    | Coding evaluation                |
| DeepMath-7B              | Mathematical solution evaluation |
| NLTK                     | NLP utilities                    |
| Pandas                   | Data processing                  |

---

# 👥 User Roles

## 👨‍🏫 Faculty (Teachers)

Faculty users can:

* Upload lecture materials (PDF)
* Generate AI-powered exam questions
* Create and manage exams
* Set exam duration and parameters
* Provide reference solutions
* Evaluate student submissions
* Detect plagiarism
* Respond to student queries
* Publish exam results

---

## 🎓 Students

Students can:

* View available exams
* Participate in timed exams
* Submit essay, coding, or mathematical answers
* View evaluation results and feedback
* Raise queries regarding grading

---

# ⚡ Core Features

## 1️⃣ AI-Based Question Generation

GenFlex automatically generates exam questions using AI.

### Essay Questions

* Extract concepts from lecture PDFs
* Use **KeyBERT** for keyword extraction
* Use **T5 transformer model** for question generation
* Context-aware question generation

### Coding Questions

* Uses curated coding problem datasets
* Retrieves relevant questions via **FAISS vector similarity search**
* Includes reference solutions

### Diverse Question Selection

* Combines embeddings for multi-topic question generation
* Generates balanced exams with varied difficulty levels

---

## 2️⃣ Automated Evaluation System

### Essay Evaluation

Essay answers are evaluated using:

* **Semantic similarity** (Sentence Transformers)
* **Concept matching** (spaCy)

**Scoring Formula**

```
Final Score =
70% Semantic Similarity +
30% Keyword/Concept Matching
```

AI-generated feedback is also provided to students.

---

### Coding Evaluation

Coding submissions are evaluated using a **fine-tuned DeepSeek model**.

Evaluation criteria:

| Metric               | Weight |
| -------------------- | ------ |
| Solution correctness | 80%    |
| Logical approach     | 10%    |
| Code structure       | 10%    |

---

### Mathematical Evaluation

Mathematical solutions are evaluated using the **DeepMath-7B model**, which analyzes:

* Step-by-step reasoning
* Mathematical correctness
* Final solution accuracy

---

## 3️⃣ Exam Management

Faculty can:

* Create, edit, and delete exams
* Publish or unpublish exams
* Set exam durations
* Generate downloadable exam PDFs
* Track student submissions

---

## 4️⃣ Lecture Summarization

GenFlex automatically summarizes uploaded lecture content using the **BART summarization model**.

Outputs include:

* Bullet-point summaries
* Key concept extraction
* Reduced content for quick review

---

## 5️⃣ Plagiarism Detection

GenFlex integrates with **Stanford MOSS** to detect plagiarism in coding submissions.

Features include:

* Cross-student code comparison
* Similarity reports
* Direct links to MOSS reports

---

## 6️⃣ Student Query System

Students can raise queries regarding evaluation results.

Features:

* Query submission
* Faculty responses
* Query status tracking
* Resolution workflow

---

## 7️⃣ PDF Exam Generation

Exams can be exported as professional PDFs using **PDFKit**, allowing instructors to maintain offline exam records.

---

# 📁 Project Structure

```
GenFlex/
│
├── public/                 # Static assets
│
├── src/                    # React Frontend
│   ├── components/
│   │   ├── common/         # Shared UI components
│   │   ├── faculty/        # Faculty features
│   │   └── student/        # Student features
│   │
│   ├── pages/              # Login, Signup, Home
│   ├── services/           # API service layer
│   ├── styles/             # Theme configuration
│   └── utils/              # Authentication utilities
│
├── backend/
│   ├── config/             # Database configuration
│   ├── controllers/        # Business logic
│   ├── middleware/         # Authentication middleware
│   ├── models/             # MongoDB schemas
│   ├── routes/             # API routes
│   └── utils/              # AI and ML utilities
│
└── mlruns/                 # MLflow experiment tracking
```

---

# 🗄 Database Models

| Model           | Description                  |
| --------------- | ---------------------------- |
| **User**        | Faculty and student accounts |
| **Exam**        | Essay-based exams            |
| **CodingExam**  | Coding assessment exams      |
| **ExamAttempt** | Student submissions          |
| **Lecture**     | Uploaded lecture materials   |
| **Query**       | Student evaluation queries   |

---

# 🔌 API Endpoints

| Endpoint               | Description                 |
| ---------------------- | --------------------------- |
| `/api/auth/*`          | Authentication routes       |
| `/api/exams/*`         | Essay exam management       |
| `/api/coding-exams/*`  | Coding exam management      |
| `/api/student/exams/*` | Student exam actions        |
| `/api/teacher/*`       | Teacher management          |
| `/api/evaluation/*`    | Evaluation services         |
| `/api/lectures/*`      | Lecture upload & management |

---

# 🔄 Key Workflows

## Exam Creation

```
Faculty Uploads Lecture PDF
        ↓
Text Extraction
        ↓
AI Generates Questions
        ↓
Faculty Reviews Questions
        ↓
Exam Stored in Database
        ↓
PDF Generated
```

---

## Exam Taking

```
Student Opens Exam
        ↓
Timer Starts
        ↓
Student Submits Answers
        ↓
Submission Stored
        ↓
Evaluation Triggered
```

---

## Evaluation Workflow

```
Teacher Triggers Evaluation
        ↓
Backend Calls Python Evaluator
        ↓
AI Model Evaluates Answers
        ↓
Score + Feedback Generated
        ↓
Results Stored in Database
```

---

# 🔐 Security Features

GenFlex implements several security mechanisms:

* **JWT Authentication** (30-day token expiration)
* **Password hashing with bcrypt**
* **Role-based access control**
* **Protected frontend routes**
* **Backend authentication middleware**

---

# 🎨 UI Features

* Fully responsive interface
* Dark and light mode support
* Real-time form validation
* Toast notifications
* Loading indicators
* Monaco code editor for coding exams
* Countdown timer for timed assessments

---

# 🛠 Development Setup

## Clone the Repository

```bash
git clone https://github.com/yourusername/GenFlex.git
cd GenFlex
```

---

## Frontend Setup

```bash
npm install
npm start
```

Frontend runs on:

```
http://localhost:3000
```

---

## Backend Setup

```bash
cd backend
npm install
npm run dev
```

Backend runs on:

```
http://localhost:5000
```

---

## Python Dependencies

Install required AI libraries:

```bash
pip install transformers torch sentence-transformers keybert spacy faiss-cpu PyPDF2 pandas nltk
python -m spacy download en_core_web_sm
```

---

# 📊 Machine Learning Experiments

GenFlex integrates **MLflow** for experiment tracking.

Tracked components include:

* Model training runs
* Evaluation metrics
* Parameter tuning
* Model artifacts

---

# 🚀 Future Improvements

Possible future enhancements include:

* Adaptive exams based on student performance
* Real-time AI feedback during exams
* Multi-language support
* Integration with LMS platforms
* AI-generated hints for students
* Advanced analytics dashboards

---

# 🤝 Contributing

Contributions are welcome.

Steps:

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to your branch
5. Open a Pull Request

---

# 📄 License

This project is licensed under the **MIT License**.

---

# 👨‍💻 Authors

Developed as part of an AI-driven educational technology project.

---

# ⭐ Acknowledgements

* HuggingFace Transformers
* PyTorch
* Stanford MOSS
* Sentence Transformers
* KeyBERT
* spaCy
* FAISS
* Chakra UI
* React

---

# 📬 Contact

For questions, suggestions, or collaboration opportunities:

**Create an issue in the repository or submit a pull request.**

---

⭐ If you like this project, consider **starring the repository**!
