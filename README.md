# Tracalorie 2.0

Tracalorie 2.0 is a modern web application that allows users to track their daily caloric intake. This project provides functionality to set daily calorie limits, add meals and workouts, calculate caloric gain or loss, and view detailed statistics.

## Table of Contents
- [Features](#features)
- [Stacks Used](#stacks-used)
- [How It Works](#how-it-works)
- [Setup and Usage](#setup-and-usage)
- [Code Explanation](#code-explanation)

## Features
- Set a daily calorie limit.
- Track meals and workouts with caloric values.
- View stats like calories consumed, burned, remaining, and progress.
- Add, filter, and remove meals and workouts.
- Reset all data for a new day.

## Stacks Used
### Frontend
- **HTML5**: Markup structure of the application.
- **CSS3**: Styling with Bootstrap for responsive design and FontAwesome for icons.
- **JavaScript (ES6)**: Interactive features and dynamic updates.

### Libraries/Frameworks
- **Bootstrap**: For responsive design and modal functionality.
- **FontAwesome**: For icons.

### Storage
- **Local Storage**: Persistent storage for calorie limits, meals, and workouts.

## How It Works
1. **Calorie Limit**: Users set a daily calorie limit through a modal form.
2. **Add Meals and Workouts**: Meals and workouts can be added with names and calorie values.
3. **Statistics Display**:
   - Total Calories: Shows net gain or loss.
   - Calories Consumed, Burned, and Remaining: Updated dynamically.
   - Progress Bar: Visualizes the remaining calorie allowance.
4. **Filter and Reset**:
   - Filter meals and workouts using input fields.
   - Reset the day to clear all data and start fresh.

## Setup and Usage
1. Clone or download the repository.
2. Ensure a browser supports modern JavaScript (e.g., Chrome, Edge, Firefox).
3. Open `index.html` in your browser.
4. Use the following features:
   - Click **Set Daily Limit** to set a calorie goal.
   - Add meals and workouts via the respective forms.
   - View stats and progress updates dynamically.
   - Use filters to search through meals and workouts.
   - Reset the day to start over.
## Installation
To set up this project on your local machine, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/your-repo.git
   ```

2. Navigate to the project directory:
   ```bash
   cd your-repo
   ```

3. Install the dependencies:
   ```bash
   npm install
   ```

4. Start the application:
   ```bash
   npm start
   ```

## Usage
Once the application is running:

1. Open your browser and navigate to `http://localhost:3000` (or the specified port).
2. [Provide step-by-step instructions on how to use the features of your application.]

## How to Use This Code on Your System
To use this code on your own system:

1. Ensure you have the following installed:
   - [Node.js](https://nodejs.org/) (version X.X or higher)
   - [Git](https://git-scm.com/)

2. Follow the steps in the Installation section above to set up the project locally.

3. If you wish to customize the code:
   - Open the files in your preferred code editor (e.g., VS Code).
   - Modify the files in the `src` directory to suit your needs.

4. Test your changes:
   - Run the application locally to ensure everything works as expected.

5. (Optional) Deploy the project to a server or hosting platform (e.g., [Netlify](https://www.netlify.com/), [Vercel](https://vercel.com/), or [Heroku](https://www.heroku.com/)).

## Contributing
Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch for your feature:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature-name"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

## Code Explanation
### HTML Structure
- **Header**: Displays the app title and buttons for setting a daily limit and resetting the day.
- **Stats Section**: Cards to show calorie stats (limit, total gain/loss, consumed, burned, remaining).
- **Items Section**:
  - Subsections for meals and workouts with forms to add entries.
  - Filters for searching through entries.
- **Modal**: For setting the daily calorie limit.

### JavaScript Logic
#### Class: `CalorieTracker`
- **Constructor**:
  - Initializes calorie limit, total calories, meals, and workouts from local storage.
  - Displays stats and loads stored items.
- **Methods**:
  - `loadItems()`: Displays all stored meals and workouts.
  - `addMeal(meal)`: Adds a meal to the tracker and updates stats.
  - `addWorkout(workout)`: Adds a workout and updates stats.
  - `removeMeal(id)`: Removes a meal by ID and updates stats.
  - `removeWorkout(id)`: Removes a workout by ID and updates stats.
  - `reset()`: Resets all data and clears the UI.
  - `setLimit(limit)`: Updates the daily calorie limit.

#### Local Storage
- Stores calorie limit, meals, and workouts persistently.
- Methods to save, retrieve, and update data are included.

### Dynamic Stats Update
- Stats are updated dynamically upon adding/removing meals or workouts.
- A progress bar visualizes the remaining calorie budget.

### Event Handling
- Event listeners are added for form submissions, button clicks, and input changes.
- Actions like adding meals, workouts, setting limits, and resetting data are handled via JavaScript.

---

This project is a complete solution for tracking caloric intake, offering a clean UI, intuitive functionality, and real-time updates. Enjoy using Tracalorie 2.0!
