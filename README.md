# GeoQuery

A smart system that automatically identifies and maps place names from natural language input, handling spelling variations and contextual understanding of geographical references.

## Project Demo
<div align="center">
  <video width="640" height="360" controls>
    <source src="./GeoQuery-Working.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

## Project Structure
The project consists of three main components:
- Frontend (React.js)
- Backend (Node.js)
- Flask Application (Python)

## Prerequisites
- Node.js (v14 or higher)
- Python 3.8+
- npm or yarn
- Git

## Installation Steps

### 1. Clone the Repository

```bash
git clone https://github.com/The-Watcher-1895/GeoQuery.git
cd GeoQuery
```

### 2. Download and Place Models
1. Download the models from [Google Drive](https://drive.google.com/drive/folders/1EvgDO6aA1YpB9ekQVjFNaarKFIv3IuRa?usp=drive_link)
2. Place the downloaded models in their respective folders:
   - Place `final-model.pt` in the root directory
   - Place `lstm.pt` in the root directory

### 3. Frontend Setup (GeoQuery-frontend)
```bash
cd GeoQuery-frontend
npm install
npm run dev
```

### 4. Backend Setup (GeoQuery-backend)
```bash
cd GeoQuery-backend
npm install
# Create .env file and add necessary environment variables
npm run start
```

### 5. Flask Application Setup (GeoQuery-flask)
```bash
cd GeoQuery-flask
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

## Environment Variables

### Backend (.env)
```
PORT=3000
DATABASE_URL=your_database_url
JWT_SECRET=your_jwt_secret
```

### Flask App (.env)
```
FLASK_APP=app.py
FLASK_ENV=development
```

## Running the Application

1. Start the Frontend:
```bash
cd GeoQuery-frontend
npm run dev
```

2. Start the Backend:
```bash
cd GeoQuery-backend
npm run start
```

3. Start the Flask Application:
```bash
cd GeoQuery-flask
python app.py
```

The application should now be running at:
- Frontend: http://localhost:5173
- Backend: http://localhost:3000
- Flask App: http://localhost:5000


## Features
- Automatic identification of place names
- Fuzzy matching for spelling variations
- Context-aware geographical reference processing
- Search history
- User authentication
- Interactive UI
- Support for both declarative and imperative sentences
- Geospatial data visualization
- Video preview functionality

## Tech Stack
- Frontend: React.js, Vite, TailwindCSS
- Backend: Node.js, Express
- ML Service: Flask, Python
- Models: PyTorch
