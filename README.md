# Spotify Authentication

This is a simple Node.js application that demonstrates how to implement Spotify authentication using the Spotify Web API and the passport-spotify authentication middleware.

## Getting Started
To get started with this application, you'll need to follow these steps:

1. Clone this repository to your local machine
2. Install dependencies by running npm install
3. Create a Spotify application and obtain your client ID and client secret
4. Create a .env file in the root directory of the project and add the following lines:

```
CLIENT_ID=your_client_id
CLIENT_SECRET=your_client_secret
REDIRECT_URI=http://localhost:3000/callback
```

5.vMake sure to replace your_client_id and your_client_secret with your own client ID and client secret, respectively.
6. Start the server by running npm start

Navigate to http://localhost:3000 in your web browser to view the application

## How it Works
This application uses the passport-spotify middleware to authenticate users with the Spotify Web API. When a user logs in with their Spotify credentials, the application obtains an access token and refresh token from the Spotify Web API, which are used to make requests on behalf of the user. The access token is stored in a session cookie, and the refresh token is stored in a database for later use.
The application uses the Spotify Web API to retrieve information about the user's Spotify account, including their top artists and tracks. This information is displayed on the home page of the application.
