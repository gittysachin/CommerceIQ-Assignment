# CommerceIQ: SDE-1: Home Assignment

## How to run -

```bash
  npm install
  npm start
```

## Problem Statement:

- Build a REST based JSON mock server to easily add, update, delete and access data from a JSON file.

  - Every data set should have a parent identifier (entity type), which will be used in the GET APIs.
  - Every data set should have an `ID` (Primary key)
  - ID should be immutable, error needs to be thrown if ID is tried to be mutated.
  - If you make `POST`, `PUT`, `PATCH` or `DELETE` requests, changes have to be automatically saved to store.json.
  - The `store.json` file should support multiple entity types.

    ![Schema_Look](https://lh6.googleusercontent.com/SBhwRnq6DtyHPWDDjVxGAmcuQpMaI58Y2it3z1mqNgkLOn4BIqG5KCG7WK26Y2_AvZ6kZCXlweWMTw3brJU0vUb7vnqYk6Atnc5sj6gZxZwTpQV58F6dfVg6j-oj_-ms-RM9EvlZ)

- Sample APIs to be supported by the mock server on store.json file:

  - `GET /posts`
  - `GET /posts/0`
  - `POST /posts`
  - `PUT /authors/1`
  - `PATCH /posts/1`
  - `DELETE /posts/1`

- Enable filtering at entity level :

  - `GET /posts?title=title1&author=CIQ`

- Enable sorting at entity level :

  - `GET /posts?_sort=views&_order=asc`

- Enable basic search at entity level:

  - `GET /posts?q=IQ`

- Support for `nested structures` will yield a `bonus point`.

- Treat store.json as an `empty slate` where you can add and retrieve any data.

---

## Solution:

- Language Used - JavaScript (NodeJS)

Implemented all the below **features** according to `problem statement` and code hosted on GitHub along with CI-CD pipeline (`GitHub Actions`) and `APIs` hosted on `AWS EC2 instance` for user consumption.

### Features:-

- [x] Every data set should have a parent identifier (entity type), which will be used in the GET APIs.
- [x] Every data set should have an ID (Primary key)
- [x] ID should be immutable, error needs to be thrown if ID is tried to be mutated.
- [x] If you make POST, PUT, PATCH or DELETE requests, changes have to be automatically saved to store.json.
- [x] The store.json file should support multiple entity types.
- [x] Sample APIs to be supported by the mock server on store.json file:
  ```md
  GET /posts
  GET /posts/0
  POST /posts
  PUT /authors/1
  PATCH /posts/1
  DELETE /posts/1
  ```
- [x] Enable filtering at entity level :

  - `GET /posts?title=title1&author=CIQ`

- [x] Enable sorting at entity level :

  - `GET /posts?_sort=views&_order=asc`

- [x] Enable basic search at entity level:

  - `GET /posts?q=IQ`

- [x] Support for `nested structures` will yield a `bonus point`.
- [x] Treat store.json as an empty slate where you can add and retrieve any data.
