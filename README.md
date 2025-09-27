# AI Resume Analyzer

A modern web application that provides intelligent feedback on resumes using AI-powered analysis. Built with React Router, TypeScript, and powered by Puter.js for cloud services and AI capabilities.

<img width="1222" height="907" alt="Screenshot 2025-09-27 at 20 35 38" src="https://github.com/user-attachments/assets/cc6da6f7-100f-4955-96f9-7f726862bcb8" />

<img width="1222" height="907" alt="Screenshot 2025-09-27 at 20 35 20" src="https://github.com/user-attachments/assets/96205a1d-9595-4017-af01-4fe5ce4c7b65" />

<img width="1470" height="919" alt="Screenshot 2025-09-27 at 20 37 12" src="https://github.com/user-attachments/assets/24b11ad9-6265-4a0c-8eb5-f9c516a0ee9c" />




## Overview

AI Resume Analyzer helps job seekers optimize their resumes by providing detailed feedback across multiple categories including ATS compatibility, content quality, structure, tone, and skills assessment. The application uses Claude-3.5-Sonnet AI model to analyze PDF resumes and generate actionable insights.

## Features

### Core Functionality
- PDF resume upload and processing
- AI-powered resume analysis using Claude-3.5-Sonnet
- Multi-category scoring system (ATS, Content, Structure, Tone & Style, Skills)
- Job-specific feedback based on company and role requirements
- Resume preview with PDF-to-image conversion
- Historical resume tracking and comparison

### Technical Features
- Server-side rendering with React Router
- TypeScript for type safety
- PDF.js integration for document processing
- Cloud storage and AI services via Puter.js
- Responsive design with Tailwind CSS
- Real-time feedback generation
- Secure user authentication

## Technology Stack

- **Frontend**: React 19, React Router 7, TypeScript
- **Styling**: Tailwind CSS with custom components
- **PDF Processing**: PDF.js for document rendering and conversion
- **AI Services**: Puter.js platform with Claude-3.5-Sonnet
- **Cloud Services**: Puter.js for file storage and key-value database
- **Build Tool**: Vite with React Router integration
- **Development**: Hot Module Replacement, TypeScript checking

## Getting Started

### Prerequisites
- Node.js 18 or higher
- npm or yarn package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/sohooow/ai-resume-analyzer.git
cd ai-resume-analyzer
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:5173`

### Usage

1. **Authentication**: Sign in using Puter.js authentication
2. **Upload Resume**: Navigate to the upload page and select a PDF resume
3. **Job Information**: Provide company name, job title, and job description for targeted analysis
4. **Analysis**: The AI will process your resume and provide detailed feedback
5. **Review Results**: View your overall score and category-specific recommendations
6. **Track Progress**: Access previously analyzed resumes from your dashboard

## Project Structure

```
ai-resume-analyzer/
├── app/
│   ├── components/          # Reusable UI components
│   │   ├── FileUploader.tsx
│   │   ├── Summary.tsx
│   │   ├── Details.tsx
│   │   └── ...
│   ├── lib/                 # Utility libraries
│   │   ├── puter.ts         # Puter.js integration
│   │   ├── pdf2img.ts       # PDF processing
│   │   └── utils.ts         # Helper functions
│   ├── routes/              # Application routes
│   │   ├── home.tsx
│   │   ├── upload.tsx
│   │   ├── resume.tsx
│   │   └── ...
│   └── root.tsx             # Root application component
├── constants/               # Application constants and AI prompts
├── public/                  # Static assets
│   └── pdf.worker.min.mjs   # PDF.js worker
├── types/                   # TypeScript type definitions
└── package.json
```

## AI Analysis Categories

The application provides feedback across five key areas:

- **ATS Score**: Applicant Tracking System compatibility
- **Content**: Quality and relevance of resume content
- **Structure**: Organization and formatting effectiveness
- **Tone & Style**: Professional presentation and language
- **Skills**: Technical and soft skills assessment

Each category receives a score out of 100 and includes specific recommendations for improvement.

## Development

### Available Scripts

- `npm run dev` - Start development server with HMR
- `npm run build` - Create production build
- `npm run start` - Start production server
- `npm run typecheck` - Run TypeScript type checking

### Building for Production

```bash
npm run build
```

The build artifacts will be stored in the `build/` directory.

## Deployment

### Docker Deployment

Build and run using Docker:

```bash
docker build -t ai-resume-analyzer .
docker run -p 3000:3000 ai-resume-analyzer
```

### Platform Deployment

The application can be deployed to any platform supporting Node.js applications:

- Vercel
- Netlify
- Railway
- Heroku
- AWS
- Google Cloud Platform
- Digital Ocean

## Configuration

The application uses environment variables for configuration. Create a `.env` file in the root directory:

```env
# Add any required environment variables here
```

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments

- Built with React Router framework
- AI services powered by Puter.js platform
- PDF processing using PDF.js library
- UI components styled with Tailwind CSS
