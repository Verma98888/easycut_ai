# easycut_ai
AI tool for cutting debate cards

EasyCutAI is a FastAPI-based tool that generates highlighted debate cards from online articles. The backend is written in FastAPI (`main.py`) and the frontend consists of a simple `index.html` page. 

To use the app, make sure the backend server is running locally on http://127.0.0.1:8000, because the frontend sends requests to the `/generate_card` endpoint. The backend requires Python dependencies listed in `requirements.txt`, including FastAPI, Uvicorn, Newspaper3k, NLTK, BeautifulSoup4, and Pydantic. NLTK will automatically download necessary data (`punkt`) the first time it runs. 

Simply open `index.html` in a browser while the backend is active to generate cards based on article URLs and tags. The app is intended for local development, and CORS is enabled to allow requests from the frontend. 

This setup allows anyone with access to the repository to run and test EasyCutAI on their own machine.
