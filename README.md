# Booggle Bottle Value Tracking App (Client)

## Overview
The Whiskey Bottle Value Tracker Client is the front-end part of a microservices-based application designed to provide users with up-to-date values of whiskey bottles in an easy-to-understand format. It leverages Vue 3 for a responsive and interactive user interface, displaying data through charts and graphs for better visualization. This client interacts with an API layer that fetches data from a PostgreSQL database hosted on AWS RDS, ensuring real-time accuracy and reliability.

## Features
-Real-time Data Visualization: View the latest trends in whiskey values through intuitive charts and graphs.  
-User-Friendly Interface: Built with Vue 3, the UI is designed for seamless user experience across devices.  
-Search and Filter: Easily search for specific whiskey releases and filter results based on criteria such as rarity, set, and more.  

## Getting Started

## Prerequisites
1) Node.js (Version 12.x or later)
2) NPM (Node Package Manager)

## Installation
1) Clone the repository

```bash```
Copy code
git clone <repository-url>
cd vite-project

2) Install dependencies
```bash```
Copy code
npm install

3) Environment Configuration
Create a .env file in the root directory and add the API layer's URL:

```env```
Copy code
VUE_APP_API_URL=http://booggle-api-endpoint

4) Run the application
```bash```
Copy code
npm run serve

This will start the client app in development mode, accessible via http://localhost:8080.

## Usage

Once the application is running, you can:

-Browse Bottle Values: Navigate through the app to view charts and graphs depicting whiskey bottle values.  
-Search and Filter: Use the search bar and filter options to find specific bottles or sets of interest.

## Contributing
We welcome contributions to the Booggle Whiskey Value Tracker Client! Please follow these steps to contribute:

Fork the repository.
1) Create a new branch for your feature (git checkout -b feature/NewFeature).
2) Commit your changes (git commit -m 'Add some NewFeature').
3) Push to the branch (git push origin feature/NewFeature).
4) Open a Pull Request.

## License
Distributed under the MIT License. See LICENSE for more information.

##Contact
Project Link: [\[GitHub Repository Link\]](https://github.com/anpythomas/booggle-client-vue)
Developer Contact: Please reach out to Andy Thomas
