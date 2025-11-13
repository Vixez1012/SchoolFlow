# SchoolFlow 📚

A comprehensive school task management app that helps you organize, track, and manage your academic workload efficiently.

## Features ✨

- **Task Management**: Create and organize tasks with multiple types:
  - To-Do
  - Classwork
  - Homework
  - Projects
  - Quiz
  - Test

- **Calendar Integration**: Visual calendar interface to select dates and manage tasks by day

- **Color-Coded Groups**: Create custom groups for different subjects/classes with custom colors

- **Priority Levels**: Mark tasks as Low, Medium, or High priority

- **Task Details**: Add descriptions and notes to your tasks

- **User Authentication**: Secure login and registration system

- **Responsive Design**: Works seamlessly on desktop and mobile devices

## Tech Stack 🛠️

### Frontend
- **React 18** - UI library
- **Vite** - Fast build tool and dev server
- **Zustand** - State management
- **Axios** - HTTP client
- **React Calendar** - Calendar component
- **CSS3** - Styling with custom design

### Backend
- **Node.js + Express** - Server framework
- **MongoDB** - Database
- **Mongoose** - ODM for MongoDB
- **JWT** - Authentication
- **bcryptjs** - Password hashing

## Getting Started 🚀

### Prerequisites
- Node.js (v16+)
- MongoDB (local or cloud instance)
- npm or yarn

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/Vixez1012/SchoolFlow.git
cd SchoolFlow
```

2. **Install root dependencies**
```bash
npm install
```

3. **Install backend dependencies**
```bash
cd server
npm install
cd ..
```

4. **Install frontend dependencies**
```bash
cd client
npm install
cd ..
```

### Configuration

1. **Backend setup** (create `/server/.env`)
```env
MONGODB_URI=mongodb://localhost:27017/schoolflow
PORT=5000
JWT_SECRET=your-secret-key-here
```

2. **Frontend setup** (create `/client/.env.local`)
```env
VITE_API_URL=http://localhost:5000/api
```

### Running the Application

#### Development Mode (runs both frontend and backend)
```bash
npm run dev
```

This will:
- Start the backend server on http://localhost:5000
- Start the frontend dev server on http://localhost:3000

#### Production Build
```bash
npm run build
```

## Project Structure 📁

```
SchoolFlow/
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/    # Reusable React components
│   │   ├── pages/         # Page components
│   │   ├── store/         # Zustand state management
│   │   ├── api/           # API client
│   │   ├── styles/        # CSS files
│   │   └── App.jsx        # Main app component
│   └── package.json
├── server/                # Node.js backend
│   ├── models/            # MongoDB schemas
│   ├── routes/            # API endpoints
│   ├── middleware/        # Authentication middleware
│   ├── index.js           # Entry point
│   └── package.json
├── package.json           # Root package configuration
└── README.md
```

## API Endpoints 🔌

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user

### Tasks
- `GET /api/tasks` - Get all tasks
- `GET /api/tasks/date/:date` - Get tasks for specific date
- `POST /api/tasks` - Create new task
- `PUT /api/tasks/:id` - Update task
- `DELETE /api/tasks/:id` - Delete task

### Groups
- `GET /api/groups` - Get all groups
- `POST /api/groups` - Create new group
- `PUT /api/groups/:id` - Update group
- `DELETE /api/groups/:id` - Delete group

## Usage 💡

1. **Register/Login**: Create an account or log in with existing credentials

2. **Create Groups**: Set up groups for your subjects/classes with custom colors

3. **Add Tasks**: Click "New Task" to create a task with:
   - Title and description
   - Task type (To-Do, Classwork, etc.)
   - Priority level
   - Due date
   - Associated group

4. **Manage Calendar**: Use the calendar to navigate dates and view tasks

5. **Track Progress**: Mark tasks as complete by clicking the checkbox

## Features Roadmap 🗺️

- [ ] Task recurring/recurring reminders
- [ ] Due time notifications
- [ ] Task attachments
- [ ] Sharing tasks with classmates
- [ ] Progress analytics and statistics
- [ ] Dark mode support
- [ ] Mobile app (React Native)
- [ ] Export tasks to PDF/Calendar formats

## Contributing 🤝

Contributions are welcome! Please feel free to submit a Pull Request.

## License 📄

This project is licensed under the MIT License - see the LICENSE file for details.

## Support 📧

If you have any questions or need help, please open an issue on GitHub or contact the maintainers.

---

**Made with ❤️ to help students stay organized**
