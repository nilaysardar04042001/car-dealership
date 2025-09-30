# Car Dealership — Modern rewrite


This repository is a modern rewrite of a car dealership lab app. It uses a two-tier approach:


- Backend: FastAPI (Python 3.13.7)
- Frontend: React + Vite + TypeScript + Tailwind CSS
- DB: PostgreSQL (containerized)
- Containerization: Docker + docker-compose (to be added in Step 2)


## Step 1: Bootstrap
This commit adds repository skeleton, .gitignore, backend requirements, and a sample Dockerfile.


## Run locally (quick)
1. Ensure Python 3.13.7 is installed and active.
2. Create and activate virtualenv in the `backend` folder.
3. `pip install -r backend/requirements.txt`


## Next steps
- Scaffold backend FastAPI app (app/main.py, models, routers)
- Add docker-compose to run backend + frontend + PostgreSQL
- Scaffold frontend (Vite + React + TypeScript + Tailwind)