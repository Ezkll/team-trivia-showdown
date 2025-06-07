# Capstone Project: Team Trivia Showdown

**Bond and Battle: A Customizable Multiplayer Quiz for Teams**
**Customizable Quizzes for Team Bonding**

## Problem Statement

Remote and hybrid teams often struggle with building rapport in a fun, engaging way. Generic icebreakers feel forced, and existing trivia games lack customization for team-specific content or real-time collaboration. Team Trivia Showdown solves this by letting hosts create rooms with personalized questions (e.g., about team members, company culture) and adjustable rules (categories, rounds), fostering connection through shared gameplay.

## Key Challenges / Pain Points

* **Time-Consuming Room Setup**: Hosts spend 10–15 minutes manually configuring rooms (categories, rounds, custom questions), delaying gameplay.
* **Manual Team Assignments**: Hosts must manually split players into teams (e.g., Sales vs. Engineering), leading to unbalanced groups or delays.
* **Real-Time Sync Issues**: Lag or desynchronized questions/answers due to unstable connections.
* **Score Tracking**: Hosts track scores manually, risking data loss.
* **Post-Game Insights**: No built-in review of historical performance.

## User Stories

### User Type: Host (Team Lead/HR)

* As a host, I want to create a room with custom questions so my team can learn fun facts about each other.
* As a host, I want to create a room with standard trivia questions so my team can play ready-made trivia games.
* As a host, I want to control the game pace (set rounds/questions/pause/reset rounds) to keep everyone engaged.
* As a host, I want to view past game results and top performers so I can recognize team members and improve future games.
* As a host, I want to customize or toggle celebration animations to align with my team's culture or preferences.

### User Type: Player

* As a player, I want to play in single-player mode so I can practice my trivia skills.
* As a player, I want to join a room with a code so I can compete with my team in real-time.
* As a player, I want to see funny animations when our team scores to make the game more fun.

## User Flows

### Single Player Mode

* **Start Game**: User selects "Single Player" from the main menu.
* **Select Game Mode**: Choose between standard trivia or custom questions.
* **Custom Question Management**: User can add questions individually or in bulk (e.g., upload CSV or paste multiple entries).
* **Gameplay**: Answer a series of questions within a set time limit.
* **Results**: Display score and correct answers at the end.

### Multiplayer Mode

* **Host Flow**:

  * **Create Room**: Host selects "Multiplayer" and clicks "Create Room".
  * **Select Game Mode**: Choose between standard trivia or custom questions.
  * **Configure Game**: Set game parameters (e.g., number of rounds, question categories).
  * **Share Code**: A unique room code is generated and shared with players.
  * **Start Game**: Once players join, host initiates the game.

* **Player Flow**:

  * **Join Room**: Player selects "Multiplayer" and enters the room code.
  * **Team Assignment**: Automatically or manually assigned to a team.
  * **Gameplay**: Participate in answering questions as per game rules.
  * **Results**: View team and individual scores at the end.

## Game Mechanics

### Single Player Mode

* **Select Game Mode**: Choose between standard trivia or custom questions.
* **Custom Question Management**: Add individual or bulk questions.
* **Question Presentation**: Display one question at a time with multiple-choice answers.
* **Timer**: Each question has a countdown timer.
* **Scoring**: Points awarded based on correctness and response time.
* **Feedback**: Immediate indication of correct or incorrect answers.
* **Progression**: Advance to the next question upon answering or when time expires.

### Multiplayer Mode

* **Select Game Mode**: Host chooses between standard trivia or custom questions.
* **Team Formation**: Players divided into teams either manually by the host or automatically.
* **Synchronized Questions**: All players receive the same question simultaneously.
* **Answer Submission**: Players submit answers within the time limit.
* **Scoring**: Team scores calculated based on collective correct answers and response times.
* **Leaderboards**: Real-time display of team rankings during the game.
* **Game Rounds**: Game consists of multiple rounds, each with a set number of questions.
* **Endgame**: Final scores displayed, highlighting winning team and top performers.

## Must-Have Features / Components

* **User Authentication**: Allow users to create accounts or play as guests.
* **Game Mode Selection**: Users choose between standard trivia and custom question modes in both single and multiplayer setups.
* **Custom Question Creation**: Users can create and manage question sets, supporting both single-entry and bulk-upload formats.
* **Game Lobby**: Interface for players to join games using room codes.
* **Real-Time Communication**: Ensure synchronized gameplay and updates across all players.
* **Responsive Design**: Optimize UI for various devices and screen sizes.
* **Accessibility Options**: Include features like adjustable text size and color contrast.
* **Analytics Dashboard**: Provide hosts with insights into game performance and player statistics.
* **Error Handling**: Graceful management of connectivity issues and unexpected errors.

## Impact and Benefits
### User Authentication
- **Enhanced Security & Personalization:**  
  Enables user accounts, fostering personalized experiences—such as saving game progress, customized settings, and tracking personal achievements.  
- **Seamless Guest Experience:**  
  Allowing guest access ensures lower entry barriers, encouraging quick engagement and broad participation from users who may not wish to register immediately.

### Game Mode Selection
- **Flexibility in Gameplay:**  
  Offering both standard trivia and custom question modes enables the game to cater to a diverse set of user preferences and playing styles.  
- **Broader Appeal:**  
  The choice between game modes can boost overall user engagement by appealing to those who enjoy experimenting with different trivia challenges and formats.

### Custom Question Creation
- **Tailored Content & Engagement:**  
  By allowing hosts to create and manage personalized questions—whether individually or via bulk-upload—the game becomes highly adaptable to the culture, team dynamics, and unique interests of different organizations.  
- **Enhanced Team Bonding:**  
  Personalized questions drive introspection and conversation among team members, effectively transforming standard trivia into a more meaningful, interactive experience.

### Game Lobby
- **Streamlined Session Management:**  
  An intuitive game lobby enables easy room creation, instantaneous joining via room codes, and efficient team assignments, which minimizes friction and reduces setup time.  
- **Improved User Onboarding:**  
  A clean, user-friendly lobby helps new players quickly understand the game flow and start playing, contributing significantly to overall user satisfaction.

### Real-Time Communication
- **Synchronized Gameplay:**  
  Robust real-time communication ensures that questions, answer submissions, and score updates are synchronized across all players, which is vital for maintaining fairness and competitive spirit.  
- **Increased Engagement:**  
  Instant feedback and live interactions contribute to an immersive experience, improving retention and enjoyment during fast-paced game sessions.

### Responsive Design
- **Optimal Experience Across Devices:**  
  A responsive design guarantees that users have a seamless, consistent experience on desktops, tablets, and smartphones—maximizing reach and engagement.  
- **Adaptability:**  
  Ensures that game elements, animations, and interactive components function flawlessly, irrespective of screen size or orientation, thereby reducing usability issues.

### Accessibility Options
- **Inclusive Gameplay:**  
  Features such as adjustable text size and color contrast enhance the game’s usability for players with visual impairments or other accessibility needs.  
- **Compliance & Broader Adoption:**  
  By meeting accessibility standards, the game is more likely to be embraced by diverse audiences, including organizations or markets with strict accessibility requirements.

### Analytics Dashboard
- **Data-Driven Insights:**  
  Hosts gain access to in-depth performance metrics, score trends, and participation data, enabling them to understand gameplay patterns and refine future sessions.  
- **Performance Recognition:**  
  Highlighting top performers and overall game metrics not only validates player efforts but also informs improvements and feature enhancements based on user behavior patterns.

### Error Handling
- **Robust System Stability:**  
  Proactive error handling minimizes system downtime and mitigates disruptions caused by connectivity issues or unexpected errors.  
- **User Trust and Satisfaction:**  
  A resilient system that gracefully recovers from glitches maintains high user confidence, ensuring that players remain engaged even during technical challenges.

## Tech Stack
### Frontend
React.js with TypeScript

- Component-based architecture perfect for game states and reusable UI elements
- Strong ecosystem for real-time features
- Excellent mobile responsiveness support
- TypeScript adds type safety for complex game logic

### Backend
Node.js with Express.js and TypeScript
- JavaScript everywhere reduces context switching
- Excellent WebSocket support for real-time gameplay
- Fast development cycle
- Great package ecosystem

### Real-Time Communication
Socket.IO

- Handles WebSocket connections with fallbacks
- Built-in room management (perfect for game lobbies)
- Automatic reconnection handling
- Event-based communication ideal for game actions

### Database
PostgreSQL with Prisma ORM

- Relational structure good for users, games, questions, scores
- ACID compliance for scoring integrity
- Prisma provides type-safe database queries
- Easy migrations and schema management

### Additional Tools
- Redis - Session management and temporary game state
- Tailwind CSS - Rapid responsive UI development
- React Query - Server state management
- Zod - Runtime validation for game data
- Jest + React Testing Library - Testing

# Phase 1: MVP Foundation (Core Gameplay)

**Goal:** Playable version with core trivia mechanics.

### **Project Manager**

* Define timeline and deliverables for single-player and basic multiplayer.
* Prioritize features: game lobby, question management, room code join, scoring.
* Set weekly sprint reviews and testing checkpoints.

### **Lead Developer**

* Scaffold project repo using `create-react-app` (frontend) and `express-generator` (backend).
* Define core types (e.g., `Question`, `Player`, `Room`, `GameState`) in TypeScript.
* Set up git branching strategy: `main`, `dev`, `feature/*`.

### **UI/UX Designer**

* Wireframe single-player and multiplayer flows.
* Use Tailwind for responsive layouts.
* Focus: intuitive lobby, question UI, and score reveal animations.

### **Backend Engineer**

* Create REST endpoints:
  `POST /create-room`, `POST /questions`, `GET /room/:code`.
* Integrate Prisma with PostgreSQL: models for User, Game, Question, Room, Score.
* Add session handling using Redis.

### **Frontend Engineer**

* Build lobby UI: room creation, join by code.
* Implement question display with timer.
* Add score display at game end.
* Use React Query for fetching game state and user data.

### **Game Mechanic Designer**

* Define scoring logic:
  `score = base points + (bonus for speed)`
* Handle team vs. solo scoring in code structure.
* Build round progression logic (e.g., end-of-round triggers).

### **DevOps Specialist**

* Set up dev environment using Docker Compose.
* Use GitHub Actions for CI: linting, type checks, tests.
* Deploy MVP on Render or Vercel (frontend) + Railway or Fly.io (backend).

### **Deliverables by End of Phase 1**

* Basic single-player and multiplayer support.
* Room code entry and synchronization.
* Functional scoring and leaderboard.
* Bulk question upload and management.
* MVP deployed to a test environment.

## Prompts Based on Components

### **Backend Initialization**


```
I'm building a multiplayer trivia game called "Team Trivia Showdown" using Node.js, Express, and TypeScript on Replit. Help me scaffold the backend with the following:

1. Set up Express with TypeScript support.
2. Organize the project with folders: /routes, /controllers, /types, /prisma.
3. Initialize Prisma and define schema models for:
   - Room (id, code, createdAt)
   - Question (id, roomId, text, choices, correctAnswer)
   - Player (id, name, roomId)
4. Create basic REST endpoints:
   - POST /room (create a room with a generated code)
   - GET /room/:code (fetch room by code)
   - POST /questions (add custom questions to a room)

Output working backend files and Prisma schema. Assume PostgreSQL is hosted externally (e.g., Supabase or Railway).
```

### **Backend Testing + In-Memory Room State**

```
I want to continue developing the backend for "Team Trivia Showdown" on Replit. The Express API and Prisma models are set. Today, I want to:

1. Create a JS-based in-memory store to emulate Redis for managing temporary room state (e.g., active players, current question).
2. Add a TTL cleanup mechanism to clear inactive rooms after 30 minutes.
3. Create test seed data for sample questions.
4. Write test cases using Jest or Postman to verify:
   - Room creation
   - Room lookup
   - Question submission

Help implement this room state cache and show how to integrate it into the Express middleware/controller logic.
```

### **Frontend Setup and Room UI**

```
Now I'm setting up the React frontend in Replit for "Team Trivia Showdown." It must use TypeScript and connect to my existing Express backend. Help me:

1. Scaffold a React project with TypeScript.
2. Build a host flow:
   - "Create Room" button that sends POST request to /room
   - Display returned room code
3. Build a player flow:
   - "Join Room" form that sends GET request to /room/:code
   - Display error if room not found
4. Use Axios or Fetch for API calls.
5. Use Zod for input validation (e.g., room code must be 6 characters).

Provide component code and file structure. Assume Tailwind is available.
```

### **Question Upload UI**

```
I'm adding question management to my React frontend for "Team Trivia Showdown." The backend supports POST /questions and links questions to a room ID. Help me:

1. Build a form to add a single question with:
   - Question text
   - 4 choices
   - Radio select for correct answer
2. Build a CSV bulk upload using papaparse:
   - Format: question,choice1,choice2,choice3,choice4,correctAnswer
3. Submit questions to the backend using Axios.
4. Display uploaded questions in a list.

Use Tailwind CSS for layout and Zod for validation. Show example form and upload handling code.
```

### **Integration and Testing**

```
I'm finishing Sprint 1 of building "Team Trivia Showdown" in Replit. I want to manually test that everything works together. Help me:

1. Test flow:
   - Host creates room → gets code
   - Player joins with code
   - Host uploads questions
   - Player can see questions (basic static screen for now)
2. Add temporary routing logic to simulate this flow in the UI.
3. Add simple toast or alert feedback for API success/failure.
4. Show me how to run smoke tests to validate all APIs are working.
5. Suggest any last cleanup before I mark Sprint 1 as complete.

Provide practical tips for debugging or testing on Replit with limited tooling.
```

---
### Risks and Assumptions
> Think About Mobile/Accessibility
> If your audience includes teams across devices or geographies, you could add a note or story on mobile responsiveness or accessibility considerations.

> The “Real-Time Sync Issues” challenge is important—consider briefly mentioning how you intend to mitigate this (e.g., WebSockets, low-latency cloud functions, etc.), or noting this as a technical consideration during development.

### Other Use Cases
> Consider a Broader Use Case
> While the current focus is on team bonding, consider mentioning that the platform could be adapted for training, onboarding, or corporate knowledge sharing, which could expand the tool’s utility and relevance to more departments (L&D, internal communications, etc.)

### Future Development (Pipeline)

