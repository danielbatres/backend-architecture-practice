# Camera Reviews System
---

## Overview: Problem to Solve
The company "RandomCameraReviews" needs a system that allows professional photographers to upload reviews of cameras. This system should enable people from anywhere in the world to search for these reviews and purchase cameras through their portal. The company has a team of frontend developers who will create a portal for editors to upload reviews, and for users to view them. As a backend specialist, your task is to provide a system, including an API, that facilitates the following:

1. Upload camera reviews.
2. Retrieve the content of reviews for display on the portal in both web and mobile versions.
3. User management specifically for editors (excluding visitors who read the reviews).

It is also known that "RandomCameraReviews" plans to focus primarily on South America, where their largest market is, but they also have sales in North America, Europe, and very few in Asia.


### Scope

#### Use Cases
* As an editor, I would like to be able to upload a camera review.
* As an editor, I would like to be able to upload a lens review for cameras.
* As an unregistered user, I would like to be able to read a review.

#### Out of Scope
* As an unregistered user, I would like to be able to upload a camera review.

---

## Architecture

### Diagrams
Include sequence diagrams, UML diagrams, etc.

### Data Model
Include entity design, JSON structures, tables, entity-relationship diagrams, etc.

---

## Limitations
* API call for uploading a review should not exceed latency limits of 500s.
* API calls for retrieving reviews for reading should have latency less than 100ms.

---

## Cost
Description/Cost analysis
Considering 1000 users who visit regularly every hour:
E.g.,
"Considering N daily users, M calls to service/database/etc."
* 1000 daily calls to serverless functions. $XX.XX
* 1000 read/write units daily to X Database on-demand. $XX.XX
Total: $xx.xx (per month/day/year)