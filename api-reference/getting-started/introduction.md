---
title: "Introduction"
description: "Overview of the TMDB API and what you can build with it"
icon: "book"
iconType: "solid"
---

<Note>
To use the TMDB API, you must first create an account and generate an API key.
Visit the [TMDB login page](https://www.themoviedb.org/login) to get started.
For questions or issues, you can also check the
[TMDB API support forum](https://www.themoviedb.org/talk/category/5047958519c29526b50017d6).
</Note>

<img
  className="block dark:hidden my-6"
  src="/images/tmdb-fav.png"
  alt="TMDB logo"
/>
<img
  className="hidden dark:block my-6"
  src="/images/tmdb-fav.png"
  alt="TMDB logo"
/>

## What is TMDB?

The Movie Database (TMDB) is a community-driven platform that provides
information about movies, TV shows, and entertainment industry professionals.

The TMDB API allows developers to programmatically access this data and
integrate it into applications such as movie discovery platforms, analytics
dashboards, and recommendation systems.

With the API, you can retrieve:
- Movie and TV show details
- Images, posters, and backdrops
- Cast and crew information
- Trending and popular content

---

## Common Use Cases

<CardGroup cols={2} className="p-6">
  <Card title="Discover movies and TV shows">
    Search for movies and TV shows by title, genre, or popularity, and display
    detailed metadata in your application.
  </Card>

  <Card title="Build recommendation features">
    Use trending and popular endpoints to suggest movies and TV shows
    to users based on current interest.
  </Card>

  <Card title="Power media applications">
    Fetch posters, backdrops, and profile images to enhance the visual
    experience of your apps and websites.
  </Card>

  <Card title="Create data-driven tools">
    Use TMDB data to build dashboards, analytics tools, or research projects
    around movies and television trends.
  </Card>
</CardGroup>

<Info>
The TMDB API registration flow is best completed on a desktop browser.
Mobile devices may not provide the best experience during setup.
</Info>

<Tip>
### Helpful tips before you begin
- Start by understanding the **authentication process**, as all API requests
  require a valid API key.
- Review the **rate limits** to avoid request throttling.
- Use the configuration endpoints to fetch supported languages, regions,
  and image base URLs.
</Tip>
