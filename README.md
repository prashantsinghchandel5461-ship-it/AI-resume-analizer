# AI-resume-analizer
# AI Resume Analyser

An AI-powered resume analysis platform that evaluates resumes against job descriptions and provides ATS-style feedback, improvement suggestions, and resume scoring.

Built using React, TypeScript, React Router v7, Tailwind CSS, and PuterJS for serverless AI processing, authentication, and cloud storage.

---

## Features

* AI-powered resume analysis
* ATS-style resume scoring
* Resume upload with PDF support
* Resume-to-image conversion for preview generation
* Job description matching
* Skill and keyword extraction
* Actionable improvement suggestions
* Authentication using PuterJS
* Serverless architecture
* Responsive modern UI
* Retry handling and caching for improved reliability

---

## Tech Stack

### Frontend

* React 19
* TypeScript
* React Router v7
* Tailwind CSS
* Vite
* Zustand

### Backend & Cloud Services

* PuterJS

  * Authentication
  * File storage
  * AI feedback generation
  * Key-value storage

### Other Libraries

* pdfjs-dist
* react-dropzone
* clsx
* tailwind-merge

---

## Project Structure

```bash
AI-Resume-Analyser-main/
│
├── app/
│   ├── components/        # Reusable UI components
│   ├── lib/               # Utility functions & Puter integration
│   ├── routes/            # Application routes/pages
│   ├── app.css            # Global styles
│   ├── root.tsx           # Root application component
│   └── routes.ts          # Route definitions
│
├── constants/             # Prompt instructions & constants
├── public/                # Static assets
├── Dockerfile             # Docker configuration
├── package.json           # Dependencies and scripts
└── README.md
```

---

## How It Works

1. User uploads a resume PDF.
2. The application converts the resume into an image preview.
3. Resume and image files are uploaded to Puter cloud storage.
4. The AI engine analyzes the resume against the provided job description.
5. ATS feedback, scores, and recommendations are generated.
6. Results are stored and displayed to the user.

---

## Application Flow

```text
User Uploads Resume
        │
        ▼
PDF Conversion & Cloud Upload
        │
        ▼
AI Resume Analysis
        │
        ▼
ATS Score & Feedback Generation
        │
        ▼
Results Dashboard
```

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/Shantanu67hy/AI-Resume-Analyser.git
cd AI-Resume-Analyser
```

### Install Dependencies

```bash
npm install
```

### Start Development Server

```bash
npm run dev
```

The application will run on:

```text
http://localhost:5173
```

---

## Available Scripts

| Command             | Description                  |
| ------------------- | ---------------------------- |
| `npm run dev`       | Start development server     |
| `npm run build`     | Build production application |
| `npm run start`     | Start production server      |
| `npm run typecheck` | Run TypeScript type checking |

---

## Environment & Configuration

This project primarily relies on PuterJS cloud services.

Ensure that:

* PuterJS services are enabled
* Internet access is available
* PDF uploads are supported in the browser

Additional environment variables can be added if custom APIs or deployments are introduced.

---

## Key Functionalities

### Resume Upload

* Drag-and-drop PDF upload
* File validation support
* Cloud-based storage

### AI Resume Evaluation

* ATS compatibility checks
* Resume scoring
* Keyword relevance analysis
* Improvement recommendations

### Performance Improvements

The application includes several optimizations:

* Retry mechanism for failed AI/file operations
* Duplicate submission prevention
* Cached analysis results
* Parallel upload and conversion pipeline
* Automatic rollback cleanup on failure

---

## Deployment

### Build the Project

```bash
npm run build
```

### Production Start

```bash
npm run start
```

### Deploy on Vercel

1. Push the repository to GitHub
2. Import the project into Vercel
3. Configure deployment settings
4. Deploy

---

## Docker Support

Build Docker image:

```bash
docker build -t ai-resume-analyser .
```

Run Docker container:

```bash
docker run -p 3000:3000 ai-resume-analyser
```

---

## Future Improvements

* Multi-format resume support
* Resume template suggestions
* AI-generated cover letters
* Resume comparison analytics
* Recruiter dashboard
* Exportable reports
* Multi-language support

---

## Screenshots

Add application screenshots here:

```text
/public/screenshots/
```

Example:

* Home Page
* Upload Page
* Analysis Dashboard
* ATS Score Summary

---

## Contributing

Contributions are welcome.

### Steps

1. Fork the repository
2. Create a new feature branch
3. Commit your changes
4. Push the branch
5. Open a pull request

---

## License

This project is licensed under the MIT License.

---

## Author

Developed by Shantanu.

GitHub Repository:

[https://github.com/Shantanu67hy/AI-Resume-Analyser](https://github.com/Shantanu67hy/AI-Resume-Analyser)
