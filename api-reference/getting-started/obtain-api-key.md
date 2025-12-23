---
title: "Obtain API Key"
description: "Learn how to generate credentials required to access the TMDB API"
icon: "key"
iconType: "solid"
---

To make requests to the TMDB API, you must authenticate using either an
**API Key** or an **Access Token (Bearer Token)**.

This guide walks you through how to generate these credentials from your
TMDB account dashboard.

---

## Step 1: Sign in to your TMDB account

Visit the [TMDB login page](https://www.themoviedb.org/login) and sign in.
If you don’t already have an account, you’ll need to create one first.

Once logged in, you’ll be redirected to your account dashboard.

<img
  className="my-6"
  src="/images/tmdb-dashboard.png"
  alt="TMDB dashboard"
/>

---

## Step 2: Open account settings

In the top-right corner of the page, click your account avatar.
From the dropdown menu, select **Settings**.

<img
  className="my-6"
  src="/images/tmdb-settings.png"
  alt="TMDB account settings"
/>

---

## Step 3: Generate your API credentials

Within the **Settings** page, navigate to the **API** section.

Scroll to the bottom of the page to find:
- **API Key (v3 auth)**
- **API Read Access Token (Bearer token)**

You can copy either credential and use it to authenticate your API requests.

<img
  className="my-6"
  src="/images/tmdb-credentials.png"
  alt="TMDB API credentials"
/>

---

<Info>
Using the **Bearer Token** is recommended when possible, as it provides a
single authentication mechanism that works across both **v3** and **v4**
TMDB API endpoints.
</Info>
