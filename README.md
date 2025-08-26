## Student Study Planner

An opinionated full-stack web app that helps students plan, track, and visualize study tasks. Built with React + Vite + TailwindCSS on the frontend and Node.js + Express + MongoDB (Mongoose) on the backend. Auth handled with JWT and bcrypt.

### Tech stack
- **Frontend**: React 19, Vite, TailwindCSS 3, React Router, Axios, Chart.js, React Big Calendar
- **Backend**: Node.js 18+, Express 5, Mongoose 8, JWT, bcrypt
- **Database**: MongoDB 7+

### How this solves a real-world problem
Students struggle to organize tasks across subjects, set priorities, and keep track of deadlines. This app provides:
- **Structured task management**: CRUD with subject, priority, status, and deadlines
- **Focus via dashboards**: Totals, pending vs completed, upcoming deadlines
- **Insights**: Progress charts and completion rates to guide planning
- **Calendar view**: Month/week/day views with drag-and-drop to reschedule tasks
- **Mobility**: Authenticated access from any device with a simple web UI

### Repository layout
```
backend/   # Express API, Mongoose models, JWT auth
frontend/  # React app (Vite), Tailwind styling, pages/components
```

### Quick start
1) Start MongoDB locally (or update MONGO_URI in backend/.env)
2) Backend
```bash
cd backend
cp .env.example .env   # if you have an example; otherwise create it per docs below
npm install
npm run dev
```
3) Frontend
```bash
cd frontend
npm install
echo "VITE_API_URL=http://localhost:5001" > .env
npm run dev
```
4) Open the app at `http://localhost:5173` (Vite will print the exact URL)

### Key Features
- **Task Management**: Create, edit, delete tasks with priority, subject, and deadlines
- **Calendar View**: Switch between list and calendar views with drag-and-drop rescheduling
- **Dashboard**: Visual progress tracking and upcoming deadlines
- **Reports**: Chart-based insights into completion rates
- **Responsive Design**: Mobile-first design that works on all devices

### Documentation
- Frontend setup and usage: see `frontend/README.md`
- Backend setup, API and models: see `backend/README.md`


