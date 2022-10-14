# Spring Boot Demo

Simple demo app providing the backend for users to complete climate challenges
and earn points.

## API
`/users`
* Get: List of users
* Put: Add a user to the list
* Delete: Delete a user

`/challenges?challenge=<CHALLENGE>&points=<POINTS>`
* Get: List of challenges that can be completed and the points per challenge
* Put: Add a challenge `<CHALLENGE>` and set the number of points `<POINTS>` rewarded
* Delete: Delete the challenge `<CHALLENGE>`

`/challenges/user/<USER>?date=<DATE>&challenge=<CHALLENGE>`
* Get: List of completed activities (filter by `<DATE>`).
* Put: Add completed challenge `<CHALLENGE>` on `<DATE>`.
* Delete: Remove a completed challenge `<CHALLENGE>` on `<DATE>`.

`/points/user/<USER>`
* Get: Total points earned by `<USER>`

## Todo
* Research documentation generation for API