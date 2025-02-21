# Max Bueckert's Stopwatch

## Existing Functionality

- **Start Button:** Initializes the clock.
- **Lap Button:** Calculates and displays the split of the last lap under the timer.
- **Reset Button:** Resets the clock and laps, while keeping it running.
- **Stop Button:** Stops the clock and shows the initial start screen.
- **Pause:** Pauses the timer, disabling lap/reset buttons.
- **Resume:** Resumes time when paused.

## Changes to Testing

- **Starts and Stops the Stopwatch:** Updated to verify that after the stop button is clicked, the initial start screen with time 00:00:00 is displayed.
- **Pauses and Resumes the Stopwatch:** Modified to extract the inner text via `.props.children` instead of `.textContent`, correcting a previous error.
- **Records and Displays Lap Times:** Altered to test the length of the lap-list following multiple clicks of the Lap Button. This change avoids the previous issue where the regex `/(\d{2}:){2}\d{2}/` also matched the running timer, leading to test errors.





https://github.com/maxbueckert/eng-intern-assessment-react-native/assets/122507377/8a715556-8d7d-4600-8c6a-3fe830b468a3

<img width="323" alt="image" src="https://github.com/maxbueckert/eng-intern-assessment-react-native/assets/122507377/ef43688e-8ac4-48f2-bfcd-61fedb0ab564">






# Technical Instructions
1. Fork this repo to your local Github account.
2. Create a new branch to complete all your work in.
3. Test your work using the provided tests
4. Create a Pull Request against the Shopify Main branch when you're done and all tests are passing

# Project Overview
The goal of this project is to implement a stopwatch application using React Native and TypeScript. The stopwatch should have the following functionality:

- Start the stopwatch to begin counting time.
- Stop the stopwatch to pause the timer.
- Displays Laps when a button is pressed.
- Reset the stopwatch to zero.

You will be provided with a basic project structure that includes the necessary files and dependencies. Your task is to write the code to implement the stopwatch functionality and ensure that it works correctly.

## Project Setup
To get started with the project, follow these steps:

1. Clone the project repository to your local development environment.

2. Install the required dependencies by running npm install in the project directory.

3. Familiarize yourself with the project structure. The main files you will be working with are:
    - /App.tsx: The main component that renders the stopwatch and handles its functionality.
    - src/Stopwatch.tsx: A separate component that represents the stopwatch display.
    - src/StopwatchButton.tsx: A separate component that represents the start, stop, and reset buttons.

4. Review the existing code in the above files to understand the initial structure and component hierarchy.

## Project Goals
Your specific goals for this project are as follows:

1. Implement the stopwatch functionality:
    - The stopwatch should start counting when the user clicks the start button.
    - The stopwatch should stop counting when the user clicks the stop button.
    - The stopwatch should reset to zero when the user clicks the reset button.
    - The stopwatch should record and display laps when user clicks the lap button.

2. Ensure code quality:
    - Write clean, well-structured, and maintainable code.
    - Follow best practices and adhere to the React and TypeScript coding conventions.
    - Pay attention to code readability, modularity, and performance.

3. Test your code:
    - Run the application and test the stopwatch functionality to ensure it works correctly.
    - Verify that the stopwatch starts, stops, resets, and records laps as expected.

4. Code documentation:
    - Document your code by adding comments and explanatory notes where necessary.
    - Provide clear explanations of the implemented functionality and any important details.

5. Version control:
    - Use Git for version control. Commit your changes regularly and push them to a branch in your forked repository.

 6. Create a Pull Request:
    - Once you have completed the project goals, create a pull request to merge your changes into the main repository.
    - Provide a clear description of the changes made and any relevant information for the code review.

## Getting Started
To start working on the project, follow these steps:

1. Clone the repository to your local development environment.

2. Install the required dependencies by running npm install in the project directory.

3. Open the project in your preferred code editor.

4. Review the existing code in the src directory to understand the initial structure and component hierarchy.

5. Implement the stopwatch functionality by modifying the necessary components (App.tsx, Stopwatch.tsx, StopwatchButton.tsx).

6. Run the application using npm start and test the stopwatch functionality.

7. Commit your changes regularly and push them to a branch in your forked repository.

8. Once you have completed the project goals, create a pull request to merge your changes into the main repository.

## Resources
Here are some resources that may be helpful during your work on this project:

- [TypeScript Documentation](https://www.typescriptlang.org/docs/) - Official documentation for TypeScript, offering guidance on TypeScript features and usage.

- [React Testing Library](https://testing-library.com/docs/react-testing-library/intro/) - Explore React Testing Library, a popular testing library for React applications.
