# API Test Scenarios

## User

### Login
- Successful sign in
- Sign in with non-existing credentials
- Sign in with empty email
- Sign in with empty password

### Registration
- Successful sign up
- Sign up with taken username
- Sign up with taken email
- Sign up with username starting from number
- Sign up with username with 41 characters
- Sign up with username containing spaces
- Sign up with empty username
- Sign up with empty email
- Sign up with invalid email format
- Sign up with empty password

### User Data
- Get current user info
- Update user image
- Update user bio
- Update username
- Update email
- Update password
- Update without authorization

---

## Articles

- Create article
- Update article
- Delete article
- Get single article
- Get all articles
- Get personal feed
- Get global feed
- Get articles by tag
- Create article without authorization
- Delete article without authorization
- Delete article of another user
- Delete non-existing article

---

## Profile

- Get profile info
- Follow user
- Unfollow user

---

## Tags

- Get tags list

---

## Comments

- Get comments
- Add comment
- Delete comment
- Delete comment of another user
- Delete comment without authorization
