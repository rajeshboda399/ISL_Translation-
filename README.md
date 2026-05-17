# ISL_Translation-
# VaaniAI — ISL Translation System

VaaniAI is a deep learning based Indian Sign Language (ISL) translation system that supports:

- ISL → Text Translation
- Text → ISL Avatar Translation
- Alphabet & Number Recognition
- Word-Level ISL Recognition
- Real-time Video Playback
- SQLite Database Integration

---

# Features

## ISL → Text

### AlphaNum Mode
- Predicts:
  - Alphabets
  - Numbers
- Input:
  - Image (.jpg, .png)
- Uses:
  - EfficientNet + PerceiverIO

### Word Mode
- Predicts:
  - ISL words
- Input:
  - Video (.mp4)
- Uses:
  - Deep learning video recognition model

---

## Text → ISL

- Converts English sentence into:
  - ISL reordered sentence
  - Gloss tokens
  - Temporal durations
  - Avatar video playback

- Uses:
  - SQLite database
  - Pre-generated avatar videos

---

# Tech Stack

## Frontend
- React
- TypeScript
- Tailwind CSS
- Vite

## Backend
- FastAPI
- PyTorch
- OpenCV
- SQLite

---

# Project Structure

```text
project/
│
├── backend/
│   ├── server.py
│   ├── model_inference.py
│   ├── database/
│   ├── models/
│   ├── videos/
│   └── requirements.txt
│
├── public/
├── src/
├── package.json


cd backend
pip install -r requirements.txt
uvicorn server:app --reload

**for frontend**
npm install
npm run dev
