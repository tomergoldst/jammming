# Jammming
Jammming is an educational React app for creating new playlists with Spotify.
build for Codecademy Web developer course as a capstone project.

![jammming](https://user-images.githubusercontent.com/19874536/87538481-f4125600-c6a4-11ea-9b10-9d50755b80e6.jpg)

## Features
- Spotify Login - the first time a user searches for a song, album, or artist, Spotify will ask them to log in or set up a new account.
- Search by Song, Album, or Artist - a user can type the name of a song, artist, or album into the search bar and click the SEARCH button.
- Populate Results List - Jammming displays the list of returned tracks from the user’s query.
- Add Song to a Custom Playlist - users can add a track to their playlist by - selecting the '+' sign on the right side of the track’s display container.
- Remove Song from Custom Playlist - users can remove a track from their playlist by selecting the '-' sign on the right side of the track’s display container.
- Change Playlist Title - users can change the title of their custom playlist.
- Save Playlist to Account - users can save their custom playlist by clicking a SAVE button.

## Instructions
In order to run this app you need to register your application using the Spotify [Application registration flow](https://developer.spotify.com/dashboard/login). Give your application a relevant name and description. Also, add the following Redirect URI: http://localhost:3000/. Once your spotify application created you will recieve your client id.

After you have a client id create a file named `apis.js` under `src\util` and define an exported variable named `spotifyClientId`. 
```js
export const spotifyClientId = 'YOUR_CLIENT_ID';
```
Run the app, In the terminal cd to the project folder and type
```shell 
npm start
```
 

## Future improvements
- Pressing enter triggers a search
- Include preview samples for each track
- Only display songs not currently present in the playlist in the search results
- Add a loading screen while playlist is saving
- Update the access token logic to expire at exactly the right time, Instead of setting expiration from when the user initiates their next search
- After user redirect on login, restoring the search term from before the redirect
- Ensure playlist information doesn’t get cleared if a user has to refresh their access token
