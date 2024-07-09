# VibeCheck
VibeCheck is a web application that uses your Spotify music taste and current location to find concerts near that you'll love. 

## How It Works
VibeCheck fetches an user's top Spotify artists using the Spotify API. The application then uses the Ticketmaster API to fetch concert events based on the user's top artists and the user's location. This allows WibeCheck to provide personalized concert recommendations based on the user's music taste and location.

## Technologies Used
- Frontend: HTML, CSS, JavaScript
- Backend: PHP
- Database: MySQL (for storing user and artist data)
- APIs: Spotify API, Ticketmaster API

## Key Features
![VibeCheck](https://github.com/kelly-tsidji/vibeCheck/assets/86772393/5f7f06c3-ca08-40e4-80e2-88e711450fac)
![VibeCheck (1)](https://github.com/kelly-tsidji/vibeCheck/assets/86772393/aff4b1a2-2959-487b-bd93-9fdb493b219f)

## Team Contributions
- Kelly T: Ticketmaster API, Password Validation
- Oliver B: Ticketmaster API, Database
- Sloan W: Spotify API, Styling
- Jackie C: Styling, Photo Slideshow

## Personal Contribution:
- Developed a dynamic event search and display feature for the website using PHP and JavaScript.
- Integrated the Ticketmaster API for real-time event data retrieval.
- Created a login system with form validation and session management to ensure secure user authentication.
- Leveraged geolocation API to personalize event recommendations based on user location.

## Database Schema
The database schema includes the following tables:
- **artists:** _ID_ (primary key), _Name_ (name of the artist), _SpotifyID_ (Spotify ID of the artist), _term_ (term associated with the artist), _pic_ (picture URL of the artist), _UserID_ (ID of the user who's top artist it is)
- **my_list:** _ID_ (primary key), _Name_ (name of the concert), _Artist_ (name of the artist), _Venue_ (venue of the concert), _Date_ (date of the concert), _Time_ (time of the concert), _City_ (city where the concert is held), _Country_ (country where the concert is held), _URL_ (URL to the concert details), ImageURL (image URL of the concert), _UserID_ (ID of the user who added) the concert
- **users:** _ID_ (primary key), _Username_ (username of the user), _Password_ (password of the user), _ImageURL_ (profile image URL of the user), _LoggedIn_ (login status of the user; 1 for logged in, 0 for logged out)
