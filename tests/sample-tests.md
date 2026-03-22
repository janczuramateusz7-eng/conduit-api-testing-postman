# Sample Postman Tests

This file contains example test scripts used in Postman to validate API responses.

---

## Status Code Validation

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

## Response Time validation

pm.test("Response time is less than 500ms", function () {
    pm.expect(pm.response.responseTime).to.be.below(500);
});

## Response Body Structure Validation

pm.test("Response contains user object", function () {
    const jsonData = pm.response.json();
    pm.expect(jsonData.user).to.exist;
});

## Token Validation

pm.test("User token exists", function () {
    const jsonData = pm.response.json();
    pm.expect(jsonData.user.token).to.exist;
});

## Error Handling Validation
pm.test("Status code is 422 for invalid data", function () {
    pm.response.to.have.status(422);
});

## Header Validation

pm.test("Content-Type is application/json", function () {
    pm.expect(pm.response.headers.get("Content-Type")).to.include("application/json");
});
