# Real-Time Location Tracking App

A real-time location tracking application built with Express.js, Node.js, and Socket.IO, using Leaflet.js for map visualization.

## Features

- Real-time location tracking
- Live updates of user locations on a map
- Handles user disconnections and updates the map accordingly

## Technologies Used

- Express.js
- Node.js
- Socket.IO
- Leaflet.js
- EJS (Embedded JavaScript templating)

## Getting Started

### Live Demo

You can see the live application running [here](https://realtime-location-tracker-qtsv.onrender.com).

### Prerequisites

Make sure you have the following installed:

- Node.js
- npm (Node package manager)

### Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/Nazeer45/RealTime_Tracker_using_ExpressJs_NodeJS.git
    cd realtime-location-tracking
    ```

2. Install the dependencies:

    ```sh
    npm install
    ```

### Running the Application

1. Start the server:

    ```sh
    npx nodemon app.js
    ```

2. Open your browser and navigate to:

    ```
    http://localhost:3000
    ```

## Project Structure

- `app.js`: The main application file that sets up the Express server, Socket.IO, and handles routing.
- `public/`: Directory for static assets like CSS and client-side JavaScript.
    - `css/style.css`: Stylesheet for the application.
    - `js/script.js`: Client-side JavaScript for handling geolocation and Socket.IO events.
- `views/index.ejs`: The EJS template for the main page.

## How It Works

1. When a user connects, their location is tracked using the Geolocation API.
2. The location data is sent to the server using Socket.IO.
3. The server broadcasts the location data to all connected clients.
4. The clients update the map with the new location data.
