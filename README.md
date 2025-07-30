# ThinkMate-StudyBuddy

ThinkMate is a web-based study tool designed to enhance learning through personalized study sessions, quizzes, flashcards, and a comprehensive dashboard. It supports students and lifelong learners by offering customizable learning preferences, AI-driven study assistance, and progress tracking.

## Table of Contents

- Features
- Installation
- Usage
- Technologies Used
  Project Structure
- Contributing


## Features

ThinkMate provides a robust set of tools to support learning:

- **Personalization Center** (`settings.html`): Customize the visual theme (Light, Dark, Blue, Green), AI personality (Professor, Mentor, Researcher, Coach), learning preferences (visual explanations, real-world examples, technical terminology), and content difficulty (Beginner to Expert).
- **Study Sessions** (`app.html`): Upload study materials (PDF or TXT), select topics (e.g., General Knowledge, AI, Science), interact with an AI buddy, and manage saved sessions.
- **Quizzes** (`quiz.html`): Generate custom quizzes with adjustable subjects, number of questions, and difficulty levels (Easy, Medium, Hard). Track scores and review results.
- **Flashcards** (`flashcards.html`): Create and study flashcard decks with options to shuffle, auto-flip, and save progress. Review performance metrics like known cards and time spent.
- **Dashboard** (`dashboard.html`): Monitor study progress (overall, concepts, history), view recent activity, manage study materials, notes, and bookmarks.
- **API Key Management**: Securely managed API keys for system integration, with options to refresh status or contact support for key rotation.

## Installation

To run ThinkMate locally, follow these steps:

1. **Clone the Repository**:

        git clone https://github.com/yourusername/thinkmate.gitcd thinkmate

    
2. **Set Up Environment**:

    - Configure API keys by contacting the system administrator (as noted in `app.html` and `quiz.html`).
    - Ensure a compatible browser (e.g., Chrome, Firefox) for optimal rendering of HTML and JavaScript.
3. **Run the Application**:

    - Host the files on a local server (e.g., using [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in VS Code or a simple HTTP server):

            npx http-server
    - Open `http://localhost:8080` in your browser and navigate to `app.html` or other pages.

## Usage

1. **Accessing the Application**:

    - Start at `app.html` for study sessions or navigate to `settings.html`, `quiz.html`, `flashcards.html`, or `dashboard.html` via the navigation bar.
    - The navigation bar, present across all pages, allows seamless switching between Study, Quiz, Flashcards, and Dashboard.
2. **Personalization**:

    - Go to `settings.html` to set your preferred visual theme, AI personality, learning preferences, and difficulty level.
    - Save preferences or reset options as needed.
3. **Study Sessions**:

    - In `app.html`, upload study materials (PDF/TXT) and select a topic to begin a learning session.
    - Interact with the AI buddy for explanations and save or load sessions for continuity.
4. **Quizzes**:

    - In `quiz.html`, configure a quiz by selecting a subject, number of questions, and difficulty.
    - Answer questions, submit responses, and review your score upon completion.
5. **Flashcards**:

    - In `flashcards.html`, create a deck by choosing a subject, number of cards, and difficulty.
    - Study cards with options to shuffle or auto-flip, and mark cards as "Known" or "Needs Review."
6. **Dashboard**:

    - In `dashboard.html`, track progress with percentage-based metrics for overall learning, concepts, and history.
    - Manage study materials, notes, and bookmarks, and review recent activity.

## Technologies Used

- **HTML5**: Core structure of the application pages (`app.html`, `settings.html`, `quiz.html`, `flashcards.html`, `dashboard.html`).
- **CSS3**: Styling for responsive and visually appealing interfaces (assumed to be in an external stylesheet, e.g., `styles.css`).
- **JavaScript**: Dynamic functionality for quiz generation, flashcard interactions, and session management (assumed to be in an external script, e.g., `script.js`).
- **Vector DB**: Referenced in `app.html` for storing study material chunks, likely powered by a backend service.
- **API Integration**: Secure API key management for system operations.

## Project Structure

    thinkmate/├── app.html # Main study session page.
              ├── settings.html # Personalization settings page.
              ├── quiz.html # Quiz creation and interaction page.
              ├── flashcards.html # Flashcard deck creation and study page.
              ├── dashboard.html # Study progress and resource management page.
        
