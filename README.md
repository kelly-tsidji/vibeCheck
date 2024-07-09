# VibeCheck
VibeCheck is a web application that uses your Spotify music taste and current location to find concerts near that you'll love. 

## How It Works
VibeCheck fetches an user's top Spotify artists using the Spotify API. The application then uses the Ticketmaster API to fetch concert events based on the user's top artists and the user's location. This allows WibeCheck to provide personalized concert recommendations based on the user's music taste and location.

## Technologies Used
- Frontend: HTML, CSS, JavaScript
- Backend: PHP
- Database: MySQL (for storing user and artist data)
- APIs: Spotify API, Ticketmaster API

## Features
![VibeCheck](https://github.com/kelly-tsidji/vibeCheck/assets/86772393/5f7f06c3-ca08-40e4-80e2-88e711450fac)
![VibeCheck (1)](https://github.com/kelly-tsidji/vibeCheck/assets/86772393/aff4b1a2-2959-487b-bd93-9fdb493b219f)


## Database Schema
The database schema includes the following tables:
- artists: ID (primary key), Name (name of the artist), SpotifyID (Spotify ID of the artist), term (term associated with the artist), pic (picture URL of the artist), UserID (ID of the user who's top artist it is)
- my_list: ID (primary key), Name (name of the concert), Artist (name of the artist), Venue (venue of the concert), Date (date of the concert), Time (time of the concert), City (city where the concert is held), Country (country where the concert is held), URL (URL to the concert details), ImageURL (image URL of the concert), UserID (ID of the user who added) the concert
- users: ID (primary key), Username (username of the user), Password (password of the user), ImageURL (profile image URL of the user), LoggedIn (login status of the user; 1 for logged in, 0 for logged out)
