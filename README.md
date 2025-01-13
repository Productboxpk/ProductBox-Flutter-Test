# ProductBox-Flutter-Test

This repository contains Flutter test designed to assess the proficiency of new applicants. The tests cover key areas such as state management, UI design, API integration, and best practices for Flutter development. Applicants are required to build a movie browsing application that integrates with an external API and Firebase for data storage and management.

## Test Overview

Create a Flutter app for a movie browsing application with the following functionalities:

1. **Movie List**: Fetch and display a list of movies in a scrollable list, with pagination support using this api /discover/movie?api_key={{apiKey}}.
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
- **Firebase Authentication**: No need to implement authentication add favorites in collection with auto-generated firebase doc-id.
  
### API Integration

- **API Documentation**: You will be using the [TheMovieDB API](https://developer.themoviedb.org/reference) for fetching movie data. Please refer to the documentation for available endpoints.
  
- **Access Tokens**:
    - **READ ACCESS TOKEN**:  
      `eyJhbGciOiJIUzI1NiJ9.eyJhdWQiOiI5OWJiNmZmNDdiMzg3N2M2ZDU5MDJhNGZjNGFlMjIzNiIsIm5iZiI6MTczNjczODI5Mi44NjcsInN1YiI6IjY3ODQ4NWY0YzgxYWNhYTYzZGJiZjFkOSIsInNjb3BlcyI6WyJhcGlfcmVhZCJdLCJ2ZXJzaW9uIjoxfQ.HNUPFo0e6aeSoTmeiULQmb4-Wd8Hv7_2fpRAXXT6Xt4`
    - **API KEY**:  
      `99bb6ff47b3877c6d5902a4fc4ae2236`
  
---

## Functional Requirements

### 1. Movie List
- Fetch a list of movies using the provided API and display them in a scrollable list.
- Implement pagination to load more movies when the user scrolls to the bottom of the list.

### 2. Movie Details
- When a movie is clicked, navigate to a detailed view showing additional information using this api /movie/939243?api_key={{api_key}}&language=en-US.

### 3. Search Functionality
- Implement a search bar to filter movies by name, this should be done on the frontend using array logics.

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
- Break down the UI into reusable widgets like:
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
- Make sure the app is responsive and works well on both phones and tablets.

---

## Submission

Once you’ve completed the task, please:

1. Push your code to a GitHub repository.
2. Ensure that all code is well-documented with meaningful comments.
3. Write clear instructions for running the app and testing the functionalities.

Good luck!
