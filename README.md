# Real-Time Location Tracker

This is a real-time location tracking app built using **Node.js**, **Express**, **Socket.IO**, and **Leaflet.js**.  
It shows the live location of all connected users on an interactive map and updates their position as they move.

## Features

- Live GPS tracking
- Real-time updates using Socket.IO
- Leaflet map with markers
- Supports multiple users at the same time
- Automatically removes markers when users disconnect

## Getting Started

### 1. Install dependencies

npm install

### 2. Start the server

npm start

shell
Copy code

### 3. Open the app

http://localhost:3000

pgsql
Copy code

## How It Works

Your browser sends your current GPS location to the server using Socket.IO.  
The server broadcasts that location to all connected clients.  
Each user is shown as a marker on the map, and their position updates live.

## Note

If you open two tabs on the same laptop, both will show the same location because they use the same GPS source.  
Use two different devices to see multiple markers in different locations.
