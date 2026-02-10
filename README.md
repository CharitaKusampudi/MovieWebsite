# Movies Website

This is a movies website built using ReactJS that fetches movie information from an API and displays a list of trending movies. The app stores the count of the trending movies and displays the most popular ones. The website is hosted on Netlify for easy deployment and sharing.

---

## Features

- Fetch movie data from an external API.
- Display trending movies based on popularity.
- Store and manage movie count for trending movies using Appwrite.
- Hosted on Netlify for seamless access.

---

## Tech Stack

- **Frontend:** ReactJS (Vite), Tailwind CSS
- **State Management:** React State (useState, useEffect)
- **Database:** Appwrite
- **API:** The Movie Database (TMDb) API (or any other movie API of your choice)

---
## 🚀 Live Demo
👉 Live URL:
https://moviewebsitewithreact.netlify.app/

---

## Getting Started

To get the project up and running on your local machine, follow these steps:


1.**Clone the Repository**: First, clone the repository to your local machine using the following command:  
git clone https://github.com/CharitaKusampudi/MovieWebsite.git

2.**Install Dependencies:** Navigate to the project directory and install the necessary dependencies using npm or yarn:
```
cd MovieWebsite
  
npm install
```
3.**Set Up Appwrite Database:**  Install and set up Appwrite by following the instructions in the Appwrite documentation. After setting up the database, make sure you configure the necessary collections and permissions.
Create a Movies collection with the required attributes (e.g., title, release date, poster, and count).

Obtain the Appwrite Project ID and API endpoint.

Configure Appwrite in the Project:

Add the Appwrite API endpoint and Project ID to the .env file:

REACT_APP_APPWRITE_API_ENDPOINT=your_appwrite_api_endpoint

REACT_APP_APPWRITE_PROJECT_ID=your_appwrite_project_id

4.**Run the Application**: Once dependencies are installed, start the app using the following command:

```
npm run dev
```

The application will be available at:http://localhost:5173

---

### App Structure

**/src**: Contains all the source files for the application.  

**/components**: Contains reusable React components used throughout the app, including:  
```
MovieCard: Displays individual movie details like title, poster, and release date.

Spinner: Shows a loading spinner while data is being fetched.

Search: Handles the search functionality for searching movies.
``` 
**/App.js**: Main app file where multiple components are integrated.

**/index.js**: Entry point to the application.

**Components:**

MovieCard: Displays individual movie details such as title, poster, and release date.

Spinner: A loading spinner displayed when fetching movie data from the API.

Search: A search bar to allow users to search for movies.

App: Main component that integrates all the features of the app and renders other components.

**Hosting on Netlify**

To deploy the project on Netlify:
- Push the code to a GitHub repository
- Log in to Netlify using GitHub
- Click New site from Git
- Select the repository
- Configure build settings:
- Build Command: npm run build
- Publish Directory: dist
- Deploy the site
- Netlify will generate a public URL that can be shared.
