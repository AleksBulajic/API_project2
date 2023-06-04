# API_project2


    # No Pay to Play

![free-to-play](https://github.com/AleksBulajic/API_project2/blob/main/images/free-to-play.png?raw=true)

This application provides a RESTful API with a front-end interface that allows users to access and explore a collection of free-to-play games. Users can browse through a list of games, search for games by genre, and add their favorite games to a personalized collection.

## Project Overview

The project aims to create a web application that utilizes the Free to Game API, which provides data on free-to-play games. The application will implement various routes to perform operations such as retrieving all free games, retrieving a specific game by its ID, adding new games, updating existing games, and deleting games. Additionally, users can add games to their favorites collection and manage their favorites.

## Technologies used
 - JavaScript 
 - MnogoDB
 - Express
 - Node.js
 - mongoose

## Heroku link
 - https://procejt2.herokuapp.com/

## Routes and Models

### Routes

- GET /games/all: Retrieves a list of all free-to-play games.
- GET /games/:id: Retrieves a specific game by its ID.
- GET /games/genre/:genre: Retrieves games based on genre.
- GET /games/title/:title Retrive game by title.
- POST /games/all: Creates a new game.
- PUT /games/:id: Updates an existing game.
- DELETE /games/:id: Deletes a game.
- POST /favorites: Allows users to add a game to their favorites.
- GET /favorites: Retrieves all games in the favorites collection.
- DELETE /favorites/:id: Deletes a game from the favorites collection.

### Models

#### Game Model

```javascript
const gamesSchema = new Schema({
  title: String,
  thumbnail: String,
  short_description: String,
  genre: String,
  platform: String,
  publisher: String,
  developer: String,
  release_date: String,
  freetogame_profile_url: String
});
```
