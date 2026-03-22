# Endpoints Tested

## User

### Login
- Method: POST
- Endpoint: /users/login
- Expected status codes:
  - 200 (success)
  - 422 (validation error)

### Register
- Method: POST
- Endpoint: /users
- Expected status codes:
  - 200 (success)
  - 422 (validation error)

### Get Current User
- Method: GET
- Endpoint: /user
- Expected status codes:
  - 200 (authorized)

### Update User
- Method: PUT
- Endpoint: /user
- Expected status codes:
  - 200 (success)
  - 401 (unauthorized)

---

## Articles

### Create Article
- Method: POST
- Endpoint: /articles
- Expected status codes:
  - 200 (success)
  - 401 (unauthorized)

### Update Article
- Method: PUT
- Endpoint: /articles/:slug
- Expected status codes:
  - 200 (success)

### Delete Article
- Method: DELETE
- Endpoint: /articles/:slug
- Expected status codes:
  - 204 (success)
  - 401 (unauthorized)
  - 403 (forbidden)
  - 404 (not found)

### Get Articles
- Method: GET
- Endpoint: /articles
- Expected status codes:
  - 200 (success)

### Get Feed
- Method: GET
- Endpoint: /articles/feed
- Expected status codes:
  - 200 (success)

---

## Profile

### Get Profile
- Method: GET
- Endpoint: /profiles/:username
- Expected status codes:
  - 200 (success)

### Follow User
- Method: POST
- Endpoint: /profiles/:username/follow
- Expected status codes:
  - 200 (success)

### Unfollow User
- Method: DELETE
- Endpoint: /profiles/:username/follow
- Expected status codes:
  - 200 (success)

---

## Tags

### Get Tags
- Method: GET
- Endpoint: /tags
- Expected status codes:
  - 200 (success)

---

## Comments

### Get Comments
- Method: GET
- Endpoint: /articles/:slug/comments
- Expected status codes:
  - 200 (success)

### Add Comment
- Method: POST
- Endpoint: /articles/:slug/comments
- Expected status codes:
  - 200 (success)

### Delete Comment
- Method: DELETE
- Endpoint: /articles/:slug/comments/:id
- Expected status codes:
  - 204 (success)
  - 401 (unauthorized)
  - 403 (forbidden)
