---
title: 'Error Codes & Rate Limits'
description: 'Below is a list of errors you may come across while using TMDB'
icon: "triangle-exclamation"
iconType: "solid"
---

## Status Codes

| Code | HTTP Status | Description |
|------|------------|------------|
| 1    | 200        | Success. |
| 2    | 501        | Invalid service: this service does not exist. |
| 3    | 401        | Authentication failed: You do not have permissions to access the service. |
| 4    | 405        | Invalid format: This service doesn't exist in that format. |
| 5    | 422        | Invalid parameters: Your request parameters are incorrect. |
| 6    | 404        | Invalid ID: The pre-requisite ID is invalid or not found. |
| 7    | 401        | Invalid API key: You must be granted a valid key. |
| 8    | 403        | Duplicate entry: The data you tried to submit already exists. |
| 9    | 503        | Service offline: This service is temporarily offline, try again later. |
| 10   | 401        | Suspended API key: Access to your account has been suspended, contact TMDB. |
| 11   | 403        | Duplicate entry: The data you tried to submit already exists. |
| 12   | 503        | Service offline: This service is temporarily offline, try again later. |
| 13   | 401        | Suspended API key: Access to your account has been suspended, contact TMDB. |
| 14   | 500        | Internal error: Something went wrong, contact TMDB. |
| 15   | 201        | The item/record was updated successfully. |
| 16   | 401        | Device denied. |
| 17   | 401        | Session denied. |
| 18   | 400        | Validation failed. |
| 19   | 406        | Invalid accept header. |
| 20   | 422        | Invalid date range: Should be a range no longer than 14 days. |

## Rate Limits

<Info>
### Legacy Rate Limits
As of December 16, 2019, the original API rate limiting (40 requests every 10 seconds) has been disabled. If you have any questions, please visit our [API support forum](https://www.themoviedb.org/talk).  
</Info>

While legacy rate limits have been disabled, we still enforce upper limits to prevent excessive bulk scraping.  
Current soft limit is around **50 requests per second**, which may change over time. Please respect this limit and heed any `429 Too Many Requests` responses.
