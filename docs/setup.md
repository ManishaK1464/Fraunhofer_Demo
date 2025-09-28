# Getting Started
Follow these quick steps to set up and run IEM-TestGen locally.

## Prerequisites
- Python 3.9 or higher  
- Node.js 16 or higher (includes npm)  
- (Optional) git
## Setup & Run

1.  extract the zip, then open a terminal: cd WEBAPP

2. Backend (FastAPI):

cd backend
python -m venv venv

Activate virtual environment:
Windows: .\venv\Scripts\activate
macOS/Linux: source venv/bin/activate
pip install -r requirements.txt

Create a .env file with:
GROQ_API_KEY=your_api_key_here
uvicorn app.main:app --reload --port 8000


3. Frontend (React/Vite):

Open a new terminal, then:
cd frontend
npm install

Create .env.local with:
VITE_API_URL=http://localhost:8000
npm run dev


4. Open browser at [http://localhost:5173](http://localhost:5173), enter requirements, and generate test cases.

---

## Notes

- Use deployed Netlify and Render URLs for production/demo.  

