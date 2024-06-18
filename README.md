Here is the corrected and simplified version of your text:

---

<h1 align="center">Flutter Developer Guide 2024</h1>


The Flutter Developer Roadmap 2023 includes **practical exercises** that cover all the essential concepts used in day-to-day development.

# Guidelines

- Before starting any practical exercises, conduct research and learn the necessary concepts.
- As you progress through the exercises, apply the new knowledge in subsequent tasks. Try to allocate a maximum of 5 days to each practical.

## Useful References

The references provided are aimed at individuals with no prior knowledge or experience in developing Flutter apps. They serve as a starting point for beginners in the field, providing basic knowledge necessary before diving into Flutter development. If you already have experience in Flutter development, you may not need to refer to the provided resources.

* [Set up Flutter Environment](https://docs.flutter.dev/get-started/install)
* [Dart Language](https://dart.dev/language)
* [Version Control with Git](https://www.udacity.com/course/version-control-with-git--ud123)
* [Layout in Flutter](https://docs.flutter.dev/ui/layout#1-select-a-layout-widget)
* [Stateful and Stateless Widgets](https://docs.flutter.dev/ui/interactive#stateful-and-stateless-widgets)
* [State Management Approaches in Flutter](https://docs.flutter.dev/data-and-backend/state-mgmt/options)
* [App Architecture in Flutter](https://medium.flutterdevs.com/design-patterns-in-flutter-part-1-c32a3ddb00e2)
* [Networking](https://docs.flutter.dev/data-and-backend/networking)
* [Asynchronous Programming](https://dart.dev/codelabs/async-await)

# Material Components

### Practical 1: Implement User Profile UI

- Display a user's profile picture, name, and bio.
- Here's [UI for reference](https://cdn.dribbble.com/userupload/5207044/file/original-ceb3338a4a693f6ab102298dd3745716.jpg?compress=1&resize=1024x768).

### Practical 2: Design a Fitness App

- Create a Flutter application and design [Static UI](https://dribbble.com/shots/21236904-Fitness-App-Design).
- The app should be responsive to different resolutions.
- Use Flutter's Material Design 3 to enhance your design process.

### Practical 3: Develop a News Application

- The home screen should show the toolbar, floating button, and news content.
- The toolbar on the screen should initially display the app's logo and title.
- As the user scrolls down to read the news, the toolbar should collapse to provide more space for the content.
  - You can use any dummy text/images as article content.
- Animate the floating button as the user scrolls down, similar to [this](https://dribbble.com/shots/3541588-Play-Button-Microinteraction).
- When the user reaches the end of the news and scrolls back up, the toolbar should re-expand and display the app's logo & title.
- You can use any images or placeholders for an eye-catching UI.
- Here's [UI for reference](https://cdn.dribbble.com/users/663782/screenshots/3742414/media/67464fde751beb373b4c6fa962edf718.gif).

### Practical 4: Implement a Survey Application

- On the Home screen, display a survey form with a question, 4 options, and a button for the next question.
  - Show progress as the user answers the questions.
- Once the survey is completed, show a pop-up message thanking the user.
  - Use an AlertDialog to thank the user.
  - The dialog will have UI to show a thank-you message, image, and button to complete the survey.
- Ask at least 3 questions with 4 options each.
- The app should ask users about their shopping experience.
- Use a `PageView` to display questions.
- You can use any images or placeholders for an eye-catching UI.
- Here's [UI for reference](https://cubicleninjas.com/wp-content/uploads/2021/01/NA-2021-Web-Questionnaire-3.jpg).

### Practical 5: Fitness Journal

- Develop an app for users to track their fitness activities.
- Use TextFields for users to input details about workout type, duration, date, and notes.
- Show all workout entries on the home screen.
- Add options to filter workout entries by date, type, and duration.
- Ensure that the app maintains entered fitness data even after device rotation.

# Navigation and Routing

### Practical 6: Implement a Leave Tracker App

- Implement an app with two screens: Home and Apply-Leave Screens.
- On the Home screen, implement UI similar to the reference.
  - Use a dummy image for the person.
  - Add a Floating Action Button on the screen.
  - On tap of the Floating Action Button, redirect the user to the Apply-Leave Screen.
- On the Apply-Leave screen:
  - Include `TextField`s for user input.
  - Add `TextField`s for the user to enter the start date, end date, and reason for the leave.
  - Add a button to apply for leave, and navigate back to the Home screen on button tap.
- Show the applied leave on the Home screen.
- The app should be responsive to different resolutions.
- You can use dummy data and any images to make the UI eye-catching.
- The app should follow material guidelines.

### Practical 7: Implement Navigation for a Messaging Application

- Implement an app using 3 screens: Onboard, Sign-in, and Home.
- On the Onboard screen, show a brief introduction to the app's features, such as messaging, voice and video calls, and file sharing.
  - Show images, titles, and subtitles to introduce app functionality.
  - Add buttons to check the next/previous features and a skip button to skip the onboarding flow.
- On the Sign-in screen, allow the user to enter their email and password, and add validation to ensure the user enters a valid email address and password.
  - Use a dummy email/password to verify user input.
- After a successful login, the user should be redirected to the Home screen.
- On the Home screen, show a screen with three tabs in the persistent bottom navigation bar.
  - Implement screens for each tab.
  - You can add any eye-catching UI.
  - The user should not be able to go back to the login screen once redirected to the Home screen (after successful login).
- The app should be responsive to different resolutions.
- You can use any images or placeholders for an eye-catching UI.
- Use [go_router](https://pub.dev/packages/go_router) for navigation.
- Here's [UI for reference](https://www.uplabs.com/posts/message-app-ui-design-d614a2fa-5f98-486d-a296-d20c1dce64f1).

### Practical 8: Implement a Color Palette App for the Web

- Implement an app using the bottom navigation bar with two tabs: Home and Palette.
- On the Home screen:
  - Display a list of tiles, each indicating a number in ascending order up to 100.
  - Each tile should be tappable, allowing the user to navigate to its detail screen.
  - On the detail screen, show the number of the list tile that the user selected.
  - The user should be able to redirect to the detail screen by passing the number in the web URL.
- On the Palette screen:
  - Display a GridList of multiple color palettes.
  - By clicking on the palette, the user should navigate to the Palette detail screen.
  - On the Palette detail screen, show a container with the selected color and add a button to favorite/unfavorite it.
- Use go_router for navigation.
- You can use any colors to make the UI eye-catching.
- Here's [UI for reference](https://www.pinterest.com/pin/844706473831200541).

# Networking

### Practical 9: Implement an Online User Directory

- The app will have

 two screens:
  - The home screen should show a list of users retrieved from an API.
  - Use a ListView to show all users.
  - Add drag-and-drop support.
  - Show a summary of users in the list, including name, image, and email.
  - Use the GET API URL: http://jsonplaceholder.typicode.com/users
- On the user-item click, display all details of the user on the next screen.
  - Use a GridView to show albums.
  - Show placeholder images for an album to make the UI eye-catching.
  - Use the GET API URL: https://jsonplaceholder.typicode.com/albums?userId=1
- Use `http` for networking.

### Practical 10: Develop a Recipe Lister Application

- Implement an app with two screens: Home & Detail.
- On the Home screen, display the list of recipes.
  - Each list item should show the recipe name and a short description.
  - Tapping a recipe should open the Recipe Detail screen.
- On the Detail screen, show full recipe details with a recipe image and description.
  - Add a back button to navigate back to the list of recipes.
- Use the GET API URL: https://yummly2.p.rapidapi.com/feeds/list
- To access the API, log in or create an account to obtain an API key.
- Use `dio` for networking.

### Practical 11: Develop an Image Saver Application

- Allow users to download an image from a given URL, display the image on the screen, and store the downloaded image file in the device's internal storage.
- The app will have one screen:
  - A text field to enter the URL.
  - Buttons to download and cancel the download.
  - Show download progress in a progress bar and notification.
  - Show the downloaded image on full screen once the download succeeds.
  - Add a button to save the downloaded images in the gallery.
- Use `dio` for networking.

### Practical 12: Implement a Drink Explorer

- Allow users to search for their favorite mocktail details.
- The app will have one screen:
  - A search bar that allows users to search for mocktails by name.
  - Use the GET API URL: https://www.thecocktaildb.com/api/json/v1/1/search.php?s={mocktail}
  - The default search text should be `mocktail`, initially showing `mocktail` in the search bar and fetching `mocktail` using the API from the search text.
- When the user taps on a mocktail, display the ingredients and details of the mocktail.
  - Use dummy data if required.

# State Management

### Practical 13: Implement a Movie Directory Application

- The app should have a persistent bottom navigation bar with two tabs: Home and Favorite.
- On the Home screen:
  - Show a list of movies in a GridView.
  - Show movie poster images in the list, including the name.
  - Use the GET API URL: https://netflix54.p.rapidapi.com
  - On tap of a movie, display all details of the movie on the next screen with a favorite button.
- On the Favorite screen:
  - Show a list of favorite movies and a button to remove them from favorites.
- Use Provider for state management and go_router for navigation.

### Practical 14: Implement a University Directory Application

- Allow users to browse and search universities from all around the world.
- On the Home screen:
  - Add a dropdown to select the country.
  - When a country is selected, display a list of universities located in that country from the API.
- Use the GET API URL: http://universities.hipolabs.com/search?country={country name}
- Use flutter_bloc for state management.

### Practical 15: Develop a Travel Application

- Implement the app with three screens.
- The Home screen should have a bottom bar with three tabs: Destinations, Search, and Settings.
- The Destinations tab should display a list of popular travel destinations with images and descriptions.
- The Search tab should allow the user to search for destinations.
  - Add a search view to search for different destinations.
  - Show a message in a TextView to notify the user when the searched destination is not available.
  - Use dummy data for destinations.
- The Settings tab should allow the user to customize app settings.
  - Add a toggle button for notifications and day/night theme settings.
- The app should preserve the state on tab change.
  - If the user scrolls to the bottom of the Destinations screen, it should preserve the scroll state across tab changes.
  - If a user searches for something on the Search screen, the search result should stay when navigating to the Search tab from other tabs.
  - If the user changes the settings toggle, it should remain as it is when the user navigates between tabs.
- Use riverpod for state management.

### Practical 16: Create a My Journal Application

- Enable users to add their daily thoughts, feelings, experiences, and ideas.
- The app will have one screen:
  - Show the user's thoughts in a grid.
  - Add a TextField to take user input.
  - Add a button to save the user's thoughts.
  - Store inputs in the state manager class as the state.
- The user should be able to add multiple thoughts.
- Use `riverpod` for state management.

### Practical 17: Develop a MathQuest Quiz Application

- The app will have one quiz screen.
- The Home screen is the entry point of the app.
  - Provide an introduction to the quiz and a button to start the quiz.
- The quiz should ask 10 questions, one at a time, and provide four answer options for each question.
  - On clicking the next button, highlight the correct/wrong answer and show the next question.
  - Show progress as the user answers the questions.
- After the user answers all questions, the app should display a result view.
  - Show the number of correct answers and the total number of questions.
  - Show the excellence level based on the score such as poor, good, and very good.
  - Add a button to restart the quiz so that the user can play again.
- Implement a day/night theme in the quiz app.
- Use any state management library for state management and images to build an eye-catching UI.
- Use injectable and getIt for dependency injection.
- Here's [UI for reference](https://cdn.dribbble.com/users/2469034/screenshots/8210470/media/f02da6249ee8c25f187432c73d4eec27.png).
- Write unit tests.

# Local Storage

### Practical 18: Develop a Protasker Application

- The app will have three screens: Login, Home, and Detail screens.
- On the Home screen:
  - Show a list of tasks with subtasks and time of creation.
  - Add a floating action button to add a new task.
  - Add a button on each cell to mark tasks as complete/incomplete.
  - On cell swipe, show the delete option and allow the user to delete it by clicking on it.
  - Display a summary of the number of pending tasks on the app bar.
  - On clicking a cell, redirect to the Task detail screen.
- On the Detail screen:
  - Allow the user to edit tasks and subtasks.
  - Add a button to save the updated data.
- Use sq_lite to store data.
- Display data from SQLite on the Home screen.
- Use any state management library.

### Practical 19: Develop Authentify

- An application that takes user credentials and basic information and navigates to the home screen after a successful login.
- The app will have one screen:
  - First, show the register form:
    - Take the user's name, email, and password for login.
    - Other basic information such as address, DOB, blood group, gender, etc.
    - Add validation for email and password.
    - Save user details in the local database.
  - After registering, show the login form:
    - Take email and password.
    - Check if the user exists. If not, notify the user to register.
    - Add validation for email.
- Once the user logs in, always show the home screen:
  - Display user details.
  - Add logout & delete user options in the toolbar.
  - Clear the user session on logout.
  - Until the user logs out, always show the home screen.
  - When the user clicks the logout/delete user button, clear/delete the user session and navigate back to the login screen.
  - Use `flutter_bloc` for state management.
  - Write unit tests for Bloc.

### Practical 20: Implement Offline-First StoreMate Product Application

- Use the GET API: https://fakestoreapi.com/products
- On the Home screen:
  - Retrieve the list of products from an API and display it to the user using a ListView.
  - Show product name, image, and a button to favorite/unfavorite the product.
- Allow the user to view the product by clicking on it:
  - Show all details of the product.
  - Add an option to favorite/unfavorite the product.
- Add an option on the Home screen to view favorite products:
  - Show all favorite products.
  - Add an option to remove from favorites.
  - Add an option to remove all favorite items.
  - Users can select multiple items with a long click and remove all selected products from their favorites.
- The application should have offline functionality, allowing the user to continue browsing products even without an internet connection.
- Fetch product data from the local database first and then sync it with remote API data.
- Add swipe-to-delete functionality to remove products from local storage.
- Add swipe-to-refresh functionality to refresh the local database with remote data.
-

 Use any state management library.
- Add unit tests.

# Streams

### Practical 21: Implement a Countdown Timer Application Using Stream

- Build an app using one screen.
- On the Home screen:
  - Add text fields to take user input for hours, minutes, and seconds.
  - Add a button to start/stop the timer.
  - Show remaining & elapsed time.
- The user should be able to set the duration of the timer and start it.
- When the timer ends, display a notification indicating that the time is up.
- Play sound and vibrate the device when the timer completes.
- Write unit tests.

### Practical 22: Implement a VocabVault App

- Allow users to search for the definition of any word in the English language.
- On the Home screen:
  - Users should be able to search for a word by typing it into a search bar.
  - Display a list of words as the user types in the search view.
  - Display the word's definition along with pronunciations, parts of speech, examples, and synonyms.
  - Add an option to play pronunciations of words.
- Make sure the app does not make unnecessary API calls while typing in the search view.
- Use StreamBuilder to render the UI.
- Use the API: https://api.dictionaryapi.dev/api/v2/entries/en/$word
- Write unit tests for the ViewModel.

# Firestore Database

### Practical 23: Develop an EmployeeHub Application

- Build an app using Google Sign-in.
- The application should have a main entry point: the Sign-in screen.
- On the Sign-in screen:
  - Display an image, introduction content, and a **Sign in with Google** button.
  - On clicking the button, authenticate the user with Google and Firebase authentication.
  - After successful sign-in, navigate the user to the Home screen.
- The application should display a list of employees on the Home screen:
  - Show basic details, including their name and job title.
- When a user clicks on an employee from the list, display their full details, including contact information, job title, and other important information.
- Allow the user to add new employees to the directory by entering their basic information and saving it locally:
  - Save employee name, email, contact info, job title, address, DOB, blood group, etc.
- Allow the user to update an employee's information by selecting them from the employee list and editing their details.
- Allow the user to delete an employee by swiping to delete from the Home screen.
- Use Firestore to store data.
- Once the user signs in successfully, redirect them to the Home screen without asking for authentication again.

### Practical 24: Create a Contact Keeper Application

- Build an app with one screen.
- On the Home screen:
  - Show all contacts, including name, phone number, and profile.
  - On clicking a contact, show the contact profile.
  - Add an option to update contact details.
  - Add an option to delete a contact by swiping to delete.
  - Add an option to add a contact with a person's name, multiple phone numbers, profile image, blood group, and address.
- Add a screen to edit/show contact details:
  - Add an option to delete a contact.
- The app should also update contacts in real-time so changes made by one user are reflected across all devices.
- Use Firestore to store contact details.
- Use rx_dart for state management.
- Write unit tests.
