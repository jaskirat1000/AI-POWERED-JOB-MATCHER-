# Resume Job Matcher - Setup Instructions

## Quick Start

### 1. Backend Setup (Terminal 1)
```bash
# Navigate to the project directory
cd resume-job-matcher-master

# Install Python dependencies
pip install -r requirements.txt

# Start the Flask backend server
python app.py
```

The backend will start on `http://localhost:5000`

### 2. Frontend Setup (Terminal 2)
```bash
# Navigate to the frontend directory
cd resume-matcher-frontend

# Install Node.js dependencies
npm install

# Start the React development server
npm start
```

The frontend will start on `http://localhost:3000`

## Testing the Setup

### Test Backend
```bash
# In the main project directory
python test_backend.py
```

### Test Frontend
1. Open `http://localhost:3000` in your browser
2. You should see the Resume Job Matcher interface
3. Try uploading a resume and enhancing a job description

## Features Fixed

✅ **File Upload**: Resumes can now be properly uploaded to the backend
✅ **Job Description Enhancement**: AI enhancement feature is working
✅ **Resume Processing**: Backend can process uploaded resumes
✅ **Frontend-Backend Integration**: Proper communication between frontend and backend

## Troubleshooting

### If backend fails to start:
- Make sure Python is installed
- Check if port 5000 is available
- Install missing dependencies: `pip install flask flask-cors werkzeug`

### If frontend fails to start:
- Make sure Node.js is installed
- Check if port 3000 is available
- Install missing dependencies: `npm install`

### If file upload doesn't work:
- Make sure both backend and frontend are running
- Check browser console for errors
- Verify the uploads folder exists

## API Endpoints

- `GET /api/health` - Health check
- `POST /api/upload-resume` - Upload a resume file
- `POST /api/process-resumes` - Process uploaded resumes
- `POST /api/enhance-job-description` - Enhance job description with AI

## File Structure

```
resume-job-matcher-master/
├── app.py                 # Flask backend
├── resume_matcher.py      # Core resume matching logic
├── uploads/              # Uploaded resume files
├── resume-matcher-frontend/  # React frontend
│   ├── src/
│   │   ├── App.tsx       # Main app component
│   │   └── components/   # React components
│   └── package.json      # Frontend dependencies
└── requirements.txt      # Backend dependencies
``` 