# 18 NoSQL: Social Network API

## Description
A REST API for a social media app. Built with Express, Mongoose, and MongoDB. REST API's are tested with Insomnia Core. 

## Walkthrough Video 

[![Watch the demo](https://img.youtube.com/vi/CAAh1RQu4YY/maxresdefault.jpg)](https://youtu.be/CAAh1RQu4YY

## User Story

```md
AS A social media startup
I WANT an API for my social network that uses a NoSQL database
SO THAT my website can handle large amounts of unstructured data
```
## Acceptance Criteria

```md
GIVEN a social network API
WHEN I enter the command to invoke the application
THEN my server is started and the Mongoose models are synced to the MongoDB database
WHEN I open API GET routes in Insomnia Core for users and thoughts
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
THEN I am able to successfully create, update, and delete users and thoughts in my database
WHEN I test API POST and DELETE routes in Insomnia Core
THEN I am able to successfully create and delete reactions to thoughts and add and remove friends to a user’s friend list
```

## Usage

1. install dependencies with npm -i
2. run npm start
3. Use insomnia core to test the API


### Models
 User
 Thoughts
 Reaction  (subdocument schema in the Thought model.)

## API Routes
User
Get all users: GET /api/users
Create a user: POST /api/users
Get user by ID: GET /api/users/:id
Update a user: PUT /api/users/:id
Delete a user: DELETE /api/users/:id
Add a friend: PUT /api/users/:userId/friends/:friendId
Delete a friend: DELETE /api/users/:userId/friends/:friendId

Thought
Get all thoughts: GET /api/thoughts
Create a thought: POST /api/thoughts
Get thought by ID: GET /api/thoughts/:id
Update a thought: PUT /api/thoughts/:id
Delete a thought: DELETE /api/thoughts/:id

Reaction
Add a reaction: PUT /api/thoughts/:id/reactions
Delete a reaction: DELETE /api/thoughts/:id/reactions

## Repository

Github link -> https://github.com/caflores31/supreme-spoon
Github Issues -> https://github.com/caflores31/supreme-spoon/issues

## Questions

For questions or queries you can send me an email caflores31@gmail.com