<p align="center">
  <img src="public/banner.png" alt="Movie Application Banner" style="border-radius:15px" width="100%">
</p>
  
<div align="center" style="margin-top:-10px;">

<br/>

<img src="https://skillicons.dev/icons?i=react&perline=1" width="90"/>

<h1>    MOVIE EXPLORER</h1>
<p><b>Find Movies You'll Enjoy</b></p>
<img src="https://img.shields.io/badge/made%20with-React%20%2B%20Appwrite-9333ea?style=for-the-badge&labelColor=0d0d0d"/>

</div>
<br/>


<br/>

# TABLE OF CONTENT
- [✨ Overview](#-overview)
- [🛠️ Tech Stack](#-tech-stack)
- [🌟 Features](#-features)
- [📂 Project Structure](#-project-structure)
- [⭐ Support](#-support)

<br/>



# ✨ Overview


<table>
<tr>
<td>

Movie Explorer is a sleek movie discovery application that allows users to search, browse trending movies, and explore detailed information powered by the TMDB API. Designed with performance, simplicity, and a clean user experience in mind, this project helped me strengthen my React fundamentals while working with real-world APIs.

</td>
</tr>
</table>



# 🛠 Tech Stack
<table>
<tr>
<td>

<div>
<img src="https://skillicons.dev/icons?i=react&perline=1"/>
<img src="https://skillicons.dev/icons?i=appwrite,nodejs,git,github&theme=dark" />
</div>


| Technology | Purpose |
|------------|----------|
|  React            | Frontend |
|  Vite | Development |
|  JavaScript | Logic |
|  CSS / Tailwind | Styling |
|  TMDB API | Movie Data |
|  Appwrite | Database |
</td>
</tr>
</table>

- **[Appwrite](https://appwrite.io/)** is an open-source Backend-as-a-Service (BaaS) platform that provides developers with a set of APIs to manage authentication, databases, storage, and more, enabling rapid development of secure and scalable applications.

- **[React.js](https://react.dev/reference/react)** is a JavaScript library developed by Meta for building user interfaces. It allows developers to create reusable UI components that manage their own state, leading to more efficient and predictable code. React is widely used for developing single-page applications (SPAs) due to its virtual DOM that improves performance and ease of maintenance.

- **[React-use](https://github.com/streamich/react-use)** is a collection of essential React hooks that simplify common tasks like managing state, side effects, and lifecycle events, promoting cleaner and more maintainable code in React applications.

- **[Tailwind CSS](https://tailwindcss.com/)** is a utility-first CSS framework that provides low-level utility classes to build custom designs without writing custom CSS, enabling rapid and responsive UI development.

- **[Vite](https://vite.dev/)** is a modern build tool that provides a fast development environment for frontend projects. It offers features like hot module replacement (HMR) and optimized builds, enhancing the development experience and performance.


<br/>

# ✨ Features

👉 **Browse All Movies**: Explore a wide range of movies available on the platform.

👉 **Search Movies**: Easily search for specific movies using a search function.

👉 **Trending Movies Algorithm**: Displays trending movies based on a dynamic algorithm.

👉 **Modern UI/UX**: A sleek and user-friendly interface designed for a great experience.

👉 **Responsiveness**: Fully responsive design that works seamlessly across devices.

and many more, including code architecture and reusability

<br/>

# 🧠 HOW THE DATA FLOWS

```
User types
   │
   ▼
useDebounce (500ms)
   │
   ▼
fetchMovies(query)
   │
   ├── query present → TMDB /search/movie
   └── no query        → TMDB /discover/movie?sort_by=popularity.desc
   │
   ▼
setMovieList(data.results)
   │
   ▼
query + results found → updateSearchCount() → Appwrite
   │
   ▼
loadTrendingMovies() → Trending rail re-renders
```

<br/>

# 🗂 PROJECT STRUCTURE

```
📦 movie-explorer
├── 📁 Components
│   ├── Search.jsx        controlled search input
│   ├── spinner.jsx        loading indicator
│   └── MovieCard.jsx       individual movie tile
├── appwrite.js             updateSearchCount() + getTrendingMovies()
├── App.jsx                 state, fetching, debounce, rendering
├── index.css               gradient text, pattern bg, layout
└── .env.local               API keys (gitignored)
```

<br/>

# ⭐ Support

If you found this project helpful,

⭐ Star the repository

🍴 Fork it

💬 Share your feedback


<div align="center">
<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>
</div>

<br/>



</div>
