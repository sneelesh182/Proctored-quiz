# Quiz Application

This is a simple quiz application built using React, Redux, and Chakra UI. The application features a timer, a quiz with multiple-choice questions, and a score page. The application also includes face detection using a webcam.

## Features

- **Navigation Bar**: The application has a navigation bar with links to the quiz and scores pages.
- **Quiz Functionality**: Users can take a quiz with multiple-choice questions. The quiz includes a timer, and users can submit their answers or skip questions.
- **Real-Time Face Detection**: A webcam feed is displayed in the quiz and scores pages to monitor the user's face.
- **Score Calculation**: The user's score is calculated based on the correct answers and displayed on the scores page.
- **Redux Integration**: The application uses Redux for state management, including loading quiz data and handling user answers.

## Technologies Used

- **React**: Frontend library for building user interfaces.
- **Redux**: State management library used to manage quiz data and user answers.
- **Chakra UI**: Component library for styling the application.
- **React Router**: Library for managing navigation between different pages.
- **Redux Thunk**: Middleware for handling asynchronous actions in Redux.
- **Redux Logger**: Middleware for logging Redux actions and state changes.
- **Webcam**: Webcam integration for face detection during the quiz.

## Getting Started

### Prerequisites

- Node.js
- npm (Node Package Manager)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/quiz-app.git
   cd quiz-app

2. Install the dependencies
    
    ``` npm i

3. Start the server

   ``` npm run dev

## Project Structure
- **Components: Contains the reusable components like Navbar.
- **Pages: Contains the main pages such as Quiz and Scores.
- **Redux: Contains the Redux-related files including actions, reducers, and store configuration.
- **App.js: The main entry point of the application.
- **Routes: Contains routing configuration.

## API Integration
The application fetches quiz data from a mock API and submits user answers to a local server API.

Quiz Data API: https://dbioz2ek0e.execute-api.ap-south-1.amazonaws.com/mockapi/get-quiz
Submit Quiz API: http://localhost:5000/api/submit-quiz

## How It Works
Navbar: Provides navigation between the Quiz and Scores pages.
Quiz: Fetches quiz data on load, starts a timer, and allows the user to answer questions. The user's answers are submitted to the backend server on completion.
Scores: Displays the user's score based on the correct answers stored in the Redux store.
