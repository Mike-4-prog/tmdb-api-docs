---
title: "Authentication"
description: "How authentication works in the TMDB API"
icon: "shield"
iconType: "solid"
---

The TMDB API uses **application-level authentication** to authorize requests.
Depending on the endpoint you are accessing, you may authenticate using:

- An **API key**
- An **Access Token** (Bearer token)
- A **session-based credential** for user-specific actions

To generate your API credentials, see the
[Obtain API Key](/api-reference/getting-started/obtain-api-key) guide.

---

## Bearer token authentication (recommended)

The most secure and flexible way to authenticate with TMDB is by using an
**API Read Access Token** as a Bearer token.

Once generated from your dashboard, include the token in the
`Authorization` request header.

```bash
curl --request GET \
  --url "https://api.themoviedb.org/3/movie/11" \
  --header "Authorization: Bearer YOUR_ACCESS_TOKEN"
```
This method works across both **v3** and **v4** TMDB API endpoints.
<Info> Bearer token authentication avoids exposing credentials in URLs and provides a single authentication flow across multiple API versions. </Info>

## Session-based authentication

Some TMDB endpoints require **user-level authentication**.
These endpoints allow users to perform actions such as:

- Rating movies and TV shows

- Managing favorites and watchlists

- Creating and editing custom lists

- These actions require a `session_id` or `guest_session_id`.

### Guest session ID

Guest sessions allow users to perform limited actions (such as rating content)
without logging in or creating a TMDB account.

Guest sessions:
- Are created using a dedicated endpoint
- Expire automatically after a short period of inactivity

### Account ID

The `account_id` uniquely identifies a TMDB user account and is required when
calling account-related endpoints.

It can be retrieved programmatically after authentication or inspected
directly when exploring account endpoints in the API reference.

<Tip>
If your application only needs to read movie or TV data, Bearer token
authentication is sufficient. Session-based authentication is only required
for user-specific actions.
</Tip>
