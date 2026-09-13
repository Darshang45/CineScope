# 🎬 CineScope

> A modern movie discovery web application built with React, powered by the TMDB API, with Appwrite-based search analytics to dynamically display trending movies.

## 🌐 Live Demo

🔗 **Live Website:** [](https://cinescope-c1zf.onrender.com)

## 📌 Overview

CineScope is a movie discovery and search web application built using React.

The application allows users to search for movies and explore popular titles. It also includes a dynamic **Trending Movies** section that uses Appwrite to track how frequently movies are searched and displays the top 5 most searched movies.

The project focuses on building a responsive React application while working with an external REST API and a backend database service.

---

## ✨ Features

- 🔍 **Movie Search**
  - Search for movies using the TMDB API.
  - Search results update based on the user's query.

- 🔥 **Trending Movies**
  - Displays the top 5 most searched movies.
  - Search frequency is tracked using Appwrite.
  - Trending movies are sorted based on search count.

- ⚡ **Debounced Search**
  - Implements search debouncing to reduce unnecessary API requests.
  - Prevents an API call from being made for every keystroke.

- 🎞️ **Movie Cards**
  - Displays movie posters and information in a clean interface.

- 📱 **Responsive UI**
  - Designed to work across different screen sizes.

- ⏳ **Loading State**
  - Displays a spinner while movie data is being fetched.

- ❌ **Error Handling**
  - Handles API and data-fetching errors gracefully.

---

## 🛠️ Tech Stack

### Frontend

- **React.js**
- **JavaScript**
- **TailwindCSS**
- **Vite**

### APIs & Backend

- **TMDB API** – Fetches movie data and search results.
- **Appwrite** – Stores search analytics and trending movie data.

### Libraries

- **React Use** – Used for implementing debounced search functionality.
- **Appwrite SDK** – Used to communicate with the Appwrite database.

---

## 🏗️ How It Works

The application uses TMDB to fetch movie data and Appwrite to track user searches.

### Movie Search Flow

```text
User enters a search query
          ↓
Debounce search input
          ↓
Send request to TMDB API
          ↓
Receive movie results
          ↓
Display movies
          ↓
Track the search in Appwrite

