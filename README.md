# ProjectFlow AI

**ProjectFlow AI** is a lightweight, browser-based project and client management workspace designed to help individuals and small teams organize projects, tasks, clients, deadlines, and project progress from a single dashboard.

It is built as a standalone HTML application using **HTML, CSS, and vanilla JavaScript**, with data persisted locally in the browser through `localStorage`.

> **Manage projects. Track tasks. Organize clients. Plan smarter.**

---

## ✨ Features

### 📊 Dashboard

The dashboard provides an overview of the workspace, including:

- Active projects
- Total clients
- Completed tasks
- Tasks currently in progress
- Upcoming deadlines
- Project progress
- Recent activity
- Project status chart

Project progress is automatically calculated from the completion status of its associated tasks.

---

### 📁 Project Management

Create and manage projects with:

- Project name
- Client
- Description
- Status
- Deadline
- Progress percentage

Supported project statuses:

- Planning
- In Progress
- Review
- Completed
- On Hold

Projects can be:

- Added
- Edited
- Deleted
- Filtered by status

The application also displays a visual progress bar for each project.

---

### ✅ Task Management

Tasks can be associated with projects and include:

- Task title
- Project
- Due date
- Priority
- Status

Supported priorities:

- Low
- Medium
- High
- Urgent

Supported task statuses:

- To Do
- In Progress
- Completed

Tasks can be created, edited, deleted, and filtered.

Project progress is automatically recalculated whenever task data changes.

---

### 👥 Client Management

Manage client information including:

- Name
- Email
- Phone
- Company
- Notes

Clients can be added, edited, and deleted directly from the application.

---

### 📅 Calendar

The Calendar section provides a monthly calendar view and highlights dates that contain project deadlines.

This makes it easier to identify upcoming project milestones and deadlines.

---

### 🤖 AI Project Planner

ProjectFlow AI includes a lightweight project planning assistant.

Users can describe a project, for example:

> "I need to build an e-commerce website for a clothing company."

The planner generates a suggested:

- Project overview
- Task list
- Milestones
- Timeline

For e-commerce or website projects, the built-in planner suggests activities such as product catalog creation, cart development, payment integration, responsive design, and SEO.

**Note:** The current implementation is a rule-based planner running locally in JavaScript; it does not connect to an external AI API.

---

### 📈 Analytics

The Analytics section provides a simple project completion overview.

It calculates the percentage of projects marked as completed and displays the result visually using a doughnut chart.

---

### 🔎 Global Search

The top navigation includes a global search field.

Search can identify matching:

- Projects
- Clients
- Tasks

The search checks project names/descriptions, client names/companies, and task titles.

---

### 🌙 Dark Mode

ProjectFlow AI supports both:

- Light mode
- Dark mode

The selected theme is saved in browser `localStorage`, so the preference can persist between sessions.

---

### ⚙️ Workspace Settings

The Settings page allows users to configure:

- Workspace name
- Display name

It also provides an option to reset the application back to its sample data.

---

## 🛠️ Technology Stack

ProjectFlow AI is intentionally simple and requires no build system.

### Frontend

- HTML5
- CSS3
- Vanilla JavaScript

### Libraries

- **Font Awesome 6** — icons
- **Chart.js 4.4.1** — charts
- **Google Fonts / Inter** — typography

These libraries are loaded through CDN links.

### Storage

Browser `localStorage` is used for application data and theme preferences.

Storage keys:

```text
projectflow_ai_data
projectflow_ai_theme
```



---

## 🚀 Getting Started

### 1. Download or clone the project

Make sure you have:

```text
index.html
```

### 2. Open the file

Simply open the HTML file in a modern web browser.

For example:

```text
Double-click → index.html
```

No:

- Node.js
- npm
- Python server
- Database
- Build process

is required.

### 3. Start managing your workspace

Use the sidebar to navigate between:

```text
Dashboard
Projects
Tasks
Clients
Calendar
AI Planner
Analytics
Settings
```

---

## 📂 Project Structure

The project is currently implemented as a single self-contained HTML file:

```text
ProjectFlow AI.html
```

The file contains:

```text
HTML
├── Application layout
├── Sidebar navigation
├── Dashboard
├── Project management
├── Task management
├── Client management
├── Calendar
├── AI Planner
├── Analytics
└── Settings

CSS
├── Light theme
├── Dark theme
├── Responsive layout
├── Cards
├── Tables
├── Forms
├── Modals
└── Navigation

JavaScript
├── Data store
├── localStorage
├── Theme management
├── Navigation
├── Search
├── Project CRUD
├── Task CRUD
├── Client CRUD
├── Calendar
├── AI Planner
└── Analytics
```

---

## 💾 Data Persistence

ProjectFlow AI stores application data locally in the browser.

The initial data contains sample:

- Clients
- Projects
- Tasks
- Workspace settings

On first launch, the application creates the default dataset and saves it to `localStorage`.

### Important

Because the application uses browser `localStorage`:

- Data is stored locally on the current browser/device.
- There is no server-side database.
- Clearing browser storage can remove application data.
- Data is not automatically synchronized between devices.

---

## 🔄 Automatic Project Progress

Project progress is calculated from completed tasks.

The calculation is essentially:

```text
Completed Tasks
---------------- × 100
Total Tasks
```

For example:

```text
5 completed tasks
10 total tasks

Progress = 50%
```

This keeps project progress connected to task completion.

---

## 📱 Responsive Design

The interface adapts to smaller screens.

On screens below approximately **900px**:

- The sidebar becomes collapsible.
- A hamburger menu is displayed.
- The main content expands to the available width.
- Dashboard cards adapt to a smaller grid.



---

## 🎨 UI Design

The application uses a modern SaaS-style interface with:

- Fixed sidebar navigation
- Rounded cards
- Soft shadows
- Status badges
- Progress bars
- Modal forms
- Responsive layouts
- Light and dark themes
- Inter typography
- Font Awesome icons

The primary visual theme uses a blue accent color with a dark navigation sidebar.

---

## 🔐 Privacy

ProjectFlow AI does not implement a backend or external application database.

Workspace data is stored in the browser using `localStorage`.

The application does load external frontend resources from CDNs:

- Google Fonts
- Font Awesome
- Chart.js



---

## ⚠️ Current Limitations

The current version is primarily a **frontend/local prototype**.

It does not currently provide:

- User authentication
- Multi-user collaboration
- Cloud database synchronization
- Server-side API
- Real-time collaboration
- External AI API integration
- Email notifications
- Calendar synchronization
- File attachments
- Cloud backups

The "AI Planner" is currently implemented using local JavaScript rules rather than a live AI service.

---

## 🔮 Future Improvements

Possible future enhancements include:

### Backend

- Node.js / Express API
- REST or GraphQL API
- PostgreSQL / MongoDB database
- User authentication
- Cloud data synchronization

### AI

- OpenAI API integration
- AI-generated project plans
- Automatic task breakdown
- Smart deadline suggestions
- Project risk detection
- AI progress summaries

### Collaboration

- Team members
- Roles and permissions
- Comments
- Activity history
- Real-time updates

### Productivity

- Drag-and-drop Kanban board
- Gantt charts
- Recurring tasks
- Notifications
- Reminders
- Time tracking

### Integrations

- Google Calendar
- Microsoft Calendar
- Slack
- Email
- Cloud storage

---

## 🧪 Sample Data

The application starts with sample workspace data including projects such as:

```text
E-commerce Website
Mobile App Redesign
Brand Identity
SEO Campaign
```

and sample clients and tasks for demonstrating the interface.



---

## 🧩 Customization

The application can be customized directly inside the HTML file.

For example, CSS variables are defined near the beginning of the stylesheet:

```css
:root {
  --bg: #f6f8fb;
  --surface: #ffffff;
  --primary: #3b5bfd;
  --text: #1a2233;
  --border: #e5e9f0;
}
```

Changing these variables makes it possible to customize the application's:

- Colors
- Backgrounds
- Borders
- Shadows
- Typography
- Overall visual identity

---

## 👨‍💻 Project Summary

**ProjectFlow AI** is a clean, standalone project-management dashboard designed as a foundation for a more advanced project and client workspace.

It demonstrates how a modern productivity application can be built using only:

```text
HTML
CSS
JavaScript
localStorage
Chart.js
Font Awesome
```

without requiring a backend or build system.

---

## ⭐ Highlights

- Modern project-management UI
- Fully browser-based
- Project CRUD
- Task CRUD
- Client management
- Deadline calendar
- Automatic project progress
- Dashboard analytics
- Search functionality
- AI-style project planner
- Light/dark mode
- Responsive design
- Local data persistence
- No build process required

---

## 📌 Version

```text
ProjectFlow AI v1.0
```

**Smart project & client workspace**
