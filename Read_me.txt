## About The Project

Study planner was created to address a massive problem students face: struggling to coordinate homework assignments, examination reviews, daily programming practice, and extracurricular activities without experiencing study fatigue or burnout.

Here's why Study planner is the last study planner you'll ever need:
* **All-in-One Dashboard:** Stop jump-switching between calendars, note-takers, and timer apps. Study planner brings your entire academic pipeline into one single-page command center.
* **Web Audio Soundscapes:** Block out distractions dynamically. Synthetic sound waves (Rain, Cafe hum, Wind, Waves) are generated directly in-browser using standard oscillators—requiring zero external MP3 downloads.
* **Workload AI Assistant:** Keeps you productive while preventing cramming. Study planner's AI Coach parses your calendar deadlines and coding stats to compute a real-time Stress Level and output customized scheduling warnings.

Of course, no one planner satisfies every single workflow. But Study planner is fully extensible, lightweight, and operates seamlessly on client-server sync patterns with offline capabilities.


### Built With

Study planner is engineered with speed and premium visual design in mind, avoiding bloated CSS libraries and build steps:

*   **HTML5** (Semantic Layout Structures)
*   **Vanilla CSS3** (Custom properties, grid alignment, glassmorphism, animations)
*   **JavaScript ES6 Modules** (State tracking, calendar construction, SVG chart rendering)
*   **Web Audio API** (In-browser noise synthesis)
*   **Node.js & Express** (Backend REST API endpoints)
*   **JSON File DB** (Persistent zero-configuration database storage)

## Getting Started

To set up a local copy of Study planner up and running inside your VS Code workspace, follow these simple steps.

### Prerequisites

You need Node.js installed to run the backend database server, and a simple HTTP server (or VS Code Live Server extension) for the ES6 modules.

* Node.js & npm:
  ```sh
  npm install npm@latest -g
  ```

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your_username/Study planner.git
   ```
2. Navigate to the backend directory and install backend packages:
   ```sh
   cd backend
   npm install
   ```
3. Start the backend Express API server:
   ```sh
   npm start
   ```
   *(Server starts at `http://localhost:3000`)*
4. Serve the frontend folder using a local HTTP server:
   ```sh
   # Open a new terminal tab in the root folder and run:
   npx http-server
   ```
   *(Frontend app serves at `http://localhost:8080`)*

## Usage

Study planner is split into five interactive workspaces:

1. **Dashboard:** Displays focus totals, streak indicators, calendar deadlines, and the active **Aether AI Coach** workload stress advisory block.
2. **Task Board:** Interactive columns (To Do, In Progress, Completed) featuring **drag-and-drop** cards, tags, checklist checkpoints, and filter bars.
3. **Academic Calendar:** A monthly grid view aggregating task assignments, exams, and logged practice events.
4. **Coding Arena:** Aggregates difficulties (Easy/Medium/Hard) and languages (Python, Rust, C++) of completed challenges, plotting completion percentages relative to weekly goals.
5. **Focus Space:** minimal full-screen Pomodoro timer linked to custom AudioContext ambient loops (Rain, Waves, Cafe hum) and volume controllers.
6. **Analytics Panel:** SVG time allocation donut charts and weekly task output trend lines.

## Functional & Non-Functional Requirements

### Functional Requirements
*   **Data Synchronization:** Updates are synced instantly to the backend Express server database.
*   **Offline Fallback Mode:** Automatically reverts to browser `localStorage` mirror cache if backend connection drops, syncing back upon reconnect.
*   **Web Audio Ambient Synthesis:** Programmatically generates audio blocks in-browser.
*   **Dynamic SVG Drawing:** Native line charts and donut graphs draw in real-time based on database contents.

### Non-Functional Requirements
*   **Sub-second Load Times:** Frontend loads in `<1.0s` by using native scripts and bypassing packaging dependencies.
*   **Usability & Aesthetics:** High-quality dark UI layouts with glowing glassmorphic panels and hardware-accelerated animations.
*   **Portability:** Runs natively in any modern browser without requiring native app packaging.


## Roadmap

- [x] Create core single-page glassmorphism layout
- [x] Implement draggable task column updates
- [x] Build browser-synthesized audio soundscapes (Rain, Cafe hum)
- [x] Add Node.js Express server API and JSON file database
- [x] Configure offline localStorage fallback synchronization
- [ ] Migrate file database to SQLite database storage
- [ ] Implement LeetCode API scraper to sync completed coding challenges automatically
- [ ] Support multiplayer collaborative study rooms via WebSockets

See the [open issues](https://github.com/your_username/repo_name/issues) for a full list of proposed features (and known issues).

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement". Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request