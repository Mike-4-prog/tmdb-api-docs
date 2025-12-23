---
title: 'Endpoints overview'
description: 'Below is an overview of all endpoints currently available on TMDB'
icon: "crosshairs"
iconType: "solid"
---

## Base URL
```
https://api.themoviedb.org/3
```

## Movies

<CardGroup cols={1}>
  <Card
    title="/search/movie"
    icon="search"
    href="http://localhost:3000/api-reference/movies/search-movies"
  >
    Search for movies by title, keyword, or phrase. Returns paginated results.
  </Card>
  <Card
    title="/movie/popular"
    icon="fire"
    href="http://localhost:3000/api-reference/movies/get-popular-movies"
  >
    Retrieve currently popular movies, updated daily based on user activity.
  </Card>
  <Card
    title="/movie/{movie_id}"
    icon="film"
    href="http://localhost:3000/api-reference/movies/get-movie-details"
  >
    Get comprehensive details for a specific movie including cast, crew, genres, and more.
  </Card>
  <Card
    title="/trending/movie/{time_window}"
    icon="chart-line"
    href="http://localhost:3000/api-reference/movies/get-trending-movies"
  >
    Retrieve trending movies based on recent user engagement.
  </Card>
  <Card
    title="/genre/movie/list"
    icon="tags"
    href="http://localhost:3000/api-reference/movies/get-movie-genres"
  >
    Get the list of official movie genres to map genre IDs to names.
  </Card>
</CardGroup>

## Lists

<CardGroup cols={1}>
  <Card
    title="/list"
    icon="plus-square"
    href="http://localhost:3000/api-reference/lists/create-list"
  >
    Create a new custom movie list. Requires write permissions.
  </Card>
  <Card
    title="/list/{list_id}"
    icon="info-circle"
    href="http://localhost:3000/api-reference/lists/get-list-details"
  >
    Retrieve detailed information about a specific movie list.
  </Card>
  <Card
    title="/list/{list_id}"
    icon="trash"
    href="http://localhost:3000/api-reference/lists/delete-list"
  >
    Permanently delete a movie list. Requires ownership and write permissions.
  </Card>
</CardGroup>
