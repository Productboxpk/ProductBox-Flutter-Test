# ProductBox-Flutter-Test

This repository contains a Flutter test designed to assess the proficiency of new applicants. The tests cover key areas such as state management, UI design, API integration, and best practices for Flutter development. Applicants are required to build a movie browsing application that integrates with an external API and Firebase for data storage and management.

---

## Test Overview

Create a Flutter app for a movie browsing application with the following functionalities:

1. **Movie List**: Fetch and display a list of movies in a scrollable list, with pagination support.
2. **Movie Details**: Display additional movie information when a movie is clicked.
3. **Favorites Management**: Allow users to mark/unmark movies as favorites and save this information in Firebase.
4. **Favorites Screen**: Display the list of favorite movies stored in Firebase.
5. **Dark/Light Theme Toggle**: Implement a theme toggle for dark and light modes.
6. **State Management**: Use **BLoC** or **Cubit** for managing the app's state.
7. **Firebase Integration**: Implement Firebase Firestore for storing favorite movies.

---

## Requirements

### Firebase Setup

- **Firebase Firestore**: Use Firebase Firestore to save and retrieve the list of favorite movies.
- **Firebase Authentication**: Firebase Authentication is not required. You can store favorites in a collection with auto-generated Firebase document IDs.

### API Integration

- **API Documentation**: You will be using the [TheMovieDB API](https://developer.themoviedb.org/reference) for fetching movie data. Please refer to the documentation for available endpoints.
  
- **Access Tokens**:
  - Create a free account on [TheMovieDB](https://www.themoviedb.org/) and get the following token and key from [API settings](https://www.themoviedb.org/settings/api):
    - **READ ACCESS TOKEN**:  
    - **API KEY**:  

---

## Functional Requirements

### 1. Movie List
- Fetch a list of movies using the provided API and display them in a scrollable list using the API endpoint:
  - `/discover/movie?api_key={{apiKey}}`
- Implement pagination to load more movies when the user scrolls to the bottom of the list.

### 2. Movie Details
- When a movie is clicked, navigate to a detailed view showing additional information using the API endpoint:
  - `/movie/{movieId}?api_key={{api_key}}&language=en-US`

### 3. Search Functionality
- Implement a search bar to filter movies by name. This should be done on the frontend using array logic.

### 4. Favorites Management
- Allow users to mark/unmark movies as favorites.
- Save favorite movies to Firebase Firestore.

### 5. Favorites Screen
- Create a separate screen to display the list of favorite movies fetched from Firebase Firestore.

### 6. Dark/Light Theme Toggle
- Implement a theme toggle that allows users to switch between light and dark themes.

---

## Firebase Integration

### 1. Firebase Setup
- Integrate Firebase into the app.
- Use Firebase Firestore to store and retrieve the favorite movie list.

### 2. Firestore Operations
- **Save Favorites**: When a user marks a movie as a favorite, store it in Firestore.
- **Fetch Favorites**: On the "Favorites" screen, fetch and display favorite movies stored in Firestore.

---

## Judging Criteria

### 1. State Management
- Use **Cubit** or **BLoC** to manage states for fetching movies, handling favorites, and managing theme settings.

### 2. Widget Reusability
- Break down the UI into reusable widgets such as:
  - `MovieCard`
  - `SearchBar`
  - `FavoriteButton`

### 3. Firebase Integration
- Properly integrate Firebase for Firestore data storage.
- Efficiently fetch and display the list of favorite movies.

### 4. Network Layer
- Design a clean, scalable network layer for fetching movie data from the API.

### 5. Bonus Points

- **Unit Testing**: Write unit tests for the **Cubit**/ **BLoC** logic.
- **Animation**: Add animations like screen transitions or a favorite toggle effect.

---

## Additional Instructions

- Use models for both Firebase and API data to ensure clean code and maintainable architecture.
- Ensure that the app handles edge cases such as empty responses, errors, and network issues gracefully.
- Make sure the app is responsive and works well on different dimension phones.

---

## Submission

Once you’ve completed the task, please:

1. Push your code to a GitHub repository.
2. Ensure that all code is well-documented with meaningful comments.
3. Write clear instructions for running the app and testing the functionalities.

Good luck!
